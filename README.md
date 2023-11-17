 # Music Player

### This is a Low-Level Design Problem

Everyone listens to songs on their favorite apps (Savvn, Wynk), but have we ever thought about how we can make our own music player? So, I have designed a music player with the features given below.

#### Assumptions
1) On reaching the end, the Next command will switch to the first song in the current playlist.
2) On reaching the start, the Back command will switch to the last song in the current playlist.
3) You can assume that songId and playlistId are always valid.
4) A song will contain the artist, album, and genre.
5) In the Add_Song and Create_playlist command, you have to create an ID by yourself.
### Features

- A user can create a playlist from an available pool of songs.
- A user can add songs to the playlist.
- User can play the playlist and be able to switch songs (forward or backward).
- List all the songs in the pool.

### Further Improvements

- We can use spring boot to make api calls in real time
- An UI can be added with this backend to work like a Music Player
- Insted of storing in memeory we can use Databases to sotore the musics



### Outcomes

- Code should be Demo-able and functionally complete.
- Code fails gracefully with a proper error message for corner/invalid cases, use exceptions for handling these cases.
- Code is be modular, try thinking in terms of Object-Oriented Design
- Input is taken from the command line or in the main function.


### Input given given from the CSV file
- ADD_SONG Song_1 Artist_1 Album_1 Genre_1

- ADD_SONG Song_2 Artist_2 Album_2 Genre_2

- ADD_SONG Song_3 Artist_3 Album_3 Genre_3

- ADD_SONG Song_4 Artist_4 Album_4 Genre_1

- ADD_SONG Song_5 Artist_5 Album_5 Genre_2

- ADD_SONG Song_6 Artist_6 Album_6 Genre_3

- ADD_SONG Song_7 Artist_7 Album_7 Genre_1

- ADD_SONG Song_8 Artist_8 Album_8 Genre_2

- ADD_SONG Song_9 Artist_9 Album_9 Genre_3

- ADD_SONG Song_10 Artist_10 Album_10 Genre_1

- LIST_SONGS

- CREATE_PLAYLIST PLAYLIST_1 2 4 6 8

- CREATE_PLAYLIST PLAYLIST_2 1 3 5 7 9

- LOAD_PLAYLIST PLAYLIST_1

- PLAY_SONG

- NEXT_SONG

- NEXT_SONG

- NEXT_SONG

- PREVIOUS_SONG

- PREVIOUS_SONG

- PREVIOUS_SONG

- PLAY_SONG

- STOP_SONG

- DELETE_PLAYLIST PLAYLIST_1

- ADD_SONG_TO_PLAYLIST PLAYLIST_2 8

- DELETE_SONG_FROM_PLAYLIST PLAYLIST_2 9

- LOAD_PLAYLIST PLAYLIST_2

- PLAY_SONG

- NEXT_SONG

- NEXT_SONG

- PREVIOUS_SONG


## Output

Song [id=1]

Song [id=2]

Song [id=3]

Song [id=4]

Song [id=5]

Song [id=6]

Song [id=7]

Song [id=8]

Song [id=9]

Song [id=10]

[Song [id=1], Song [id=2], Song [id=3], Song [id=4], Song [id=5], Song [id=6], Song [id=7], Song [id=8], Song [id=9], Song [id=10]]

Playlist [id=1]

Playlist [id=2]

Playlist PLAYLIST_1 is loaded!

Song [id=2] is playing!

Song [id=4] is playing!

Song [id=6] is playing!

Song [id=8] is playing!

Song [id=6] is playing!

Song [id=4] is playing!

Song [id=2] is playing!

Song [id=2] is paused!

Song [id=2] is stopped!

Playlist PLAYLIST_1 is deleted!

Playlist PLAYLIST_2 is revised with [Song [id=1], Song [id=3], Song [id=5], Song [id=7], Song [id=9], Song [id=8]]

Playlist PLAYLIST_2 is revised with [Song [id=1], Song [id=3], Song [id=5], Song [id=7], Song [id=8]]

Playlist PLAYLIST_2 is loaded!

Song [id=1] is playing!

Song [id=3] is playing!

Song [id=5] is playing!

Song [id=3] is playing!
