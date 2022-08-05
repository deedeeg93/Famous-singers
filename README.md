# Famous-singers

CREATE TABLE singers (id INTEGER PRIMARY KEY, name TEXT, age INTEGER, albums INTEGER, status TEXT);
INSERT INTO singers VALUES (1, "Harry Styles", 28, 2, "single");
INSERT INTO singers VALUES (2, "Ariana Grande", 28, 12, "married");
INSERT INTO singers VALUES (3, "Mario", 35, 5, "single");
INSERT INTO singers VALUES (5, "Miley Cyrus", 29,13, "single");
INSERT INTO singers VALUES (6, "Jack Harlow",24 ,2, "single");
INSERT INTO singers VALUES (7, "Adele", 34, 8, "single");
INSERT INTO singers VALUES (8, "Celine Dion", 54, 46, "married");

CREATE TABLE countries (id INTEGER PRIMARY KEY, name TEXT, country TEXT);

INSERT INTO countries VALUES (1, "Harry Styles", "UK");
INSERT INTO countries VALUES (2, "Ariana Grande", "USA");
INSERT INTO countries VALUES (3, "Mario", "USA");
INSERT INTO countries VALUES (4, "Alexis Jordan", "USA");
INSERT INTO countries VALUES (5, "Miley Cyrus", "USA");
INSERT INTO countries VALUES (6, "Jack Harlow", "USA");
INSERT INTO countries VALUES (7, "Adele", "UK");
INSERT INTO countries VALUES (8, "Celine Dion", "Canada");


SELECT name, age FROM singers;

SELECT * FROM singers WHERE (age >25);
SELECT * FROM singers WHERE (albums >6);

SELECT name FROM countries WHERE (country ="USA");
SELECT name FROM countries WHERE (country= "UK");

SELECT * FROM singers WHERE(status= "married" OR albums>=5);
SELECT * FROM singers WHERE(status= "single" OR albums<=4);
