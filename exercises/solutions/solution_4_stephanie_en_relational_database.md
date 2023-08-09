## Creating the various tables 
### Create the tables Users, Post, Comment, and Category
* CREATE TABLE Users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    email VARCHAR(50) UNIQUE NOT NULL,
    bio VARCHAR(50)  NOT NULL,
    password VARCHAR(50) NOT NULL
);

* CREATE TABLE Category (
    id INT PRIMARY KEY,
    name VARCHAR(50) UNIQUE NOT NULL
);

* CREATE TABLE Post (
    id INT PRIMARY KEY,
    title VARCHAR(100) NOT NULL,
    content TEXT NOT NULL,
    user_id INT NOT NULL,
    category_id INT NOT NULL,
    likes INT DEFAULT 0,
    dislikes INT DEFAULT 0,
    FOREIGN KEY (user_id) REFERENCES Users(id),
    FOREIGN KEY (category_id) REFERENCES Category(id)
);

* CREATE TABLE Comment (
    id INT PRIMARY KEY,
    content TEXT NOT NULL,
    user_id INT NOT NULL,
    post_id INT NOT NULL,
    likes INT DEFAULT 0,
    dislikes INT DEFAULT 0,
    FOREIGN KEY (user_id) REFERENCES Users(id),
    FOREIGN KEY (post_id) REFERENCES Post(id)
);

## Writing some SQL queries to perform various tasks on the database
### Query 1: Find all posts by a given user
    SELECT * FROM Post
    WHERE user_id = 1; 

### Query 2: Find all comments on a given post
    SELECT * FROM Comment
    WHERE post_id = 1;

### Query 3: Find all posts that have at least one comment
    SELECT * FROM Post 
    JOIN Comment  ON Post.id = Comment.post_id
    GROUP BY Post.id;

### Query 4: Find all categories and their number of posts
    SELECT Category.name, COUNT(Post.id) AS num_posts FROM Category 
    LEFT JOIN Post Post ON Category.id = Post.category_id
    GROUP BY Category.id;

### Query 5: Find all users and their number of likes and dislikes
    SELECT Users.name, SUM(Post.likes + Comment.likes) AS total_likes, SUM(Post.dislikes + Comment.dislikes) AS total_dislikes FROM Users 
    LEFT JOIN Post ON Users.id = Post.user_id
    LEFT JOIN Comment ON Users.id = Comment.user_id
    GROUP BY Users.id

