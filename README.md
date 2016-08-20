# Python_SQLite
Work1: Pass XML file into DB
  Schema:
  CREATE TABLE Artist (
      id  INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE,
      name    TEXT UNIQUE
  );

  CREATE TABLE Genre (
      id  INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE,
      name    TEXT UNIQUE
  );

  CREATE TABLE Album (
      id  INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE,
      artist_id  INTEGER,
      title   TEXT UNIQUE
  );

  CREATE TABLE Track (
      id  INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE,
      title TEXT  UNIQUE,
      album_id  INTEGER,
      genre_id  INTEGER,
      len INTEGER,
      rating INTEGER,
      count INTEGER
  );
