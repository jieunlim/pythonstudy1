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



