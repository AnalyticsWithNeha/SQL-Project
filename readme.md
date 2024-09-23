# Music Database

This repository contains SQL scripts for creating and populating a music database. The database consists of multiple tables that store information about artists, albums, genres, tracks, and playlists.

## Database Structure

The database consists of the following tables:

1. **Artist**
   - `artist_id` (INT): Unique identifier for each artist
   - `artist_name` (VARCHAR): Name of the artist

2. **Genre**
   - `genre_id` (INT): Unique identifier for each genre
   - `genre_name` (VARCHAR): Name of the genre

3. **Albums**
   - `album_id` (INT): Unique identifier for each album
   - `album_name` (VARCHAR): Name of the album
   - `artist_id` (INT): Foreign key referencing the artist
   - `release_date` (DATE): Release date of the album

4. **Tracks**
   - `track_id` (INT): Unique identifier for each track
   - `track_name` (VARCHAR): Name of the track
   - `album_id` (INT): Foreign key referencing the album
   - `genre_id` (INT): Foreign key referencing the genre
   - `duration` (TIME): Duration of the track

5. **Playlists**
   - `playlist_id` (INT): Unique identifier for each playlist
   - `playlist_name` (VARCHAR): Name of the playlist
   - `creation_date` (DATE): Creation date of the playlist

6. **PlaylistTracks**
   - `playlist_id` (INT): Foreign key referencing the playlist
   - `track_id` (INT): Foreign key referencing the track

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AnalyticsWithNeha/SQL-Project.git
   cd music_db
2. Create the database and tables by executing the SQL script in a MySQL environment.

## Contributing
Contributions are welcome! If you'd like to improve the analysis or add new features, feel free to fork the repository and submit a pull request.

## Licence
### Licence Information:
MIT LICENCE

## Contact
### Author:
Neha Chauhan
analyticswithneha@gmail.com