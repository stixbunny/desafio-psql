CREATE DATABASE movies;

\c movies
CREATE TABLE movie (
  id SERIAL,
  name VARCHAR(50)
  );

INSERT INTO TABLE movie (name) VALUES ('El Rey Leon');

INSERT INTO TABLE movie (name) VALUES ('Terminator 2');

ALTER TABLE movie ADD COLUMN year INTEGER;

ALTER TABLE movie ADD COLUMN genre VARCHAR(20);

UPDATE movie SET year=1984;

UPDATE movie SET genre='Drama';

DELETE FROM movie WHERE name='Terminator 2';

INSERT INTO TABLE movie (name) VALUES ('Crimen Ferpecto');
