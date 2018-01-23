# pythonstudy1

show databases;

use test;

show tables;

select count(*) from user_score;

DROP TABLE user_score;

CREATE TABLE user_score (

id int AUTO_INCREMENT primary key,

    first_name varchar(32),
    last_name varchar(32),
    score int default 0,
    created timestamp DEFAULT CURRENT_TIMESTAMP
);

INSERT INTO user_score (first_name, last_name, score) VALUES ('keeyong','han', 100);

INSERT INTO user_score (first_name, last_name, score) VALUES ('nathan','hou', 90);

INSERT INTO user_score (first_name, last_name, score) VALUES ('james','sullins', 80);

INSERT INTO user_score (first_name, last_name, score) VALUES ('paul','williams', 70);

INSERT INTO user_score (first_name, last_name) VALUES ('sarah','williams');

select * from user_score;
<a href="https://imgur.com/a2f1u7t"><img src="https://i.imgur.com/a2f1u7t.png" title="source: imgur.com" /></a>

select last_name, AVG(score), MIN(score), MAX(score) from user_score GROUP BY last_name;
<a href="https://imgur.com/2jLL3XP"><img src="https://i.imgur.com/2jLL3XP.png" title="source: imgur.com" /></a>

select last_name, AVG(score), MIN(score), MAX(score) from user_score GROUP BY 1 ORDER BY 2 DESC;
<a href="https://imgur.com/2jLL3XP"><img src="https://i.imgur.com/2jLL3XP.png" title="source: imgur.com" /></a>

select last_name from user_score;
<a href="https://imgur.com/5Wzm9Qz"><img src="https://i.imgur.com/5Wzm9Qz.png" title="source: imgur.com" /></a>

select distinct (last_name) from user_score;
<a href="https://imgur.com/UNbHpIa"><img src="https://i.imgur.com/UNbHpIa.png" title="source: imgur.com" /></a>



