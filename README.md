# Experiment 4: Displaying Dynamic Content (Read Operations)

## 📌 Overview
This project displays dynamic content fetched from MySQL using Node.js and EJS.  
A list of blog posts is shown with title, content, author name, and creation date.

---

## 📁 Folder Structure

---

## 🗄️ Database Setup

Run the SQL script (`sql/posts.sql`):

```sql
CREATE TABLE posts (
    id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(255),
    content TEXT,
    author_id INT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

INSERT INTO posts (title, content, author_id) VALUES
('First Blog Post', 'This is the first blog post content.', 1),
('Node.js Tutorial', 'Learn Node.js step by step.', 1),
('Web Development Tips', 'Some useful tips for web developers.', 2);
