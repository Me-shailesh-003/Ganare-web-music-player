Ganare, a cool music website where you can listen to all your favourite songs.

With the slogan "Ganare, where melodies reflect the soul,"

ganare is a simple and user-friendly music web player catering to music enthusiasts. this platform
enables users to enjoy seamless song playback, navigate through songs (next/previous), pause/play,
and download songs via an intuitive song player.


Here the information of database : 

CREATE DATABASE gana_bajao;
USE gana_bajao;

CREATE TABLE admin_info (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL,
    password VARCHAR(255) NOT NULL
);

CREATE TABLE user_info (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL,
    password VARCHAR(255) NOT NULL,
    phone_number VARCHAR(15) NOT NULL,
    language VARCHAR(20) NOT NULL,
    gender VARCHAR(10) NOT NULL,
    age INT NOT NULL
);

CREATE TABLE song (
    id INT AUTO_INCREMENT PRIMARY KEY,
    song_name VARCHAR(255) NOT NULL,
    singer_name VARCHAR(255),
    language VARCHAR(50),
    release_year INT,
    album_name VARCHAR(255),
    image_filename VARCHAR(255),
    audio_filename VARCHAR(255)
);

CREATE TABLE playlists (
    id INT AUTO_INCREMENT PRIMARY KEY,
    playlistName VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL
);

