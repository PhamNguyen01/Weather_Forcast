# Weather forecast Website

## Analyze the interface

The main interface of the website includes the following main components:

- Map
- Left toolbar:
  + Menu (preferred weather, weather alerts)
  + Search
  + Share
- Info tool on the right:
  + Log out
  + zoom in/out the map
  + Hello user
- Icons add map layer

## API: 
- "fed32be58df3a0bd09ff4c02c0da7443"
- "527afe48950c282cf057bbcd097c6aff"
- "c9c8e558cd1dad0583f2600da8c72b7e"
- "41fb46afccd1a8c36210e21fb8e28471"

Step 1: Create and Insert into Database, Using MySQL through Xampp:

CREATE TABLE users (
  id INT(11) NOT NULL AUTO_INCREMENT,
  username VARCHAR(50) NOT NULL,
  password VARCHAR(255) NOT NULL,
  email VARCHAR(100) NOT NULL,
  PRIMARY KEY (id)
);

INSERT INTO users (username, password, email) VALUES ('johndoe', 'password', 'johndoe@example.com');

CREATE TABLE user_favorites (
  id INT(11) NOT NULL AUTO_INCREMENT,
  user_id INT(11) NOT NULL,
  weather_type VARCHAR(50) NOT NULL,
  region VARCHAR(50) NOT NULL,
  PRIMARY KEY (id),
  FOREIGN KEY (user_id) REFERENCES users(id)
);

CREATE TABLE user_favorites (
  id INT(11) NOT NULL AUTO_INCREMENT,
  user_id INT(11) NOT NULL,
  weather_type VARCHAR(50) NOT NULL,
  region VARCHAR(50) NOT NULL,
  PRIMARY KEY (id),
  FOREIGN KEY (user_id) REFERENCES users(id)
);

Step 2: Import package:

- pip install mysql-connector-python
- pip install Flask
- pip install flask-cors

Step 3: How to run?

- runing Xampp, turn on Apache and MySQL
- runing main.py
- runing main.html with live server
