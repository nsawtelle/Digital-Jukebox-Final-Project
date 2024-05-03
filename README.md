# Digital Jukebox Final Project

Nicole Sawtelle
----

This python program simulates a digital jukebox capable of managing playlists and playback controls. It includes classes to represent songs, playlists, and the jukebox itself. The playlists are implemented using doubly linked lists to allow efficient traversal and manipulation of songs.

Doubly linked lists are a type of linked list in which each node contains a pointer to the previous node as well as the next node of the linked list. Advantages of doubly linked lists include: forwards and backwards list traversal, it is quick to insert a new node before a given node. Additionally, in a singly linked list, to delete a node, a pointer to the previous node is needed, which might require the list to be traversed. In doubly linked lists, we can get the previous node using the previous pointer. Disadvantages of doubly linked lists include: all operations require an extra pointer previous to be maintained. For example, in insertion, we need to modify previous pointers together with the next pointers.

----
The program uses 4 classes:
1. Song, which represents a song with attributes such as title, artist, and duration.
2. Node, which represents a node in a doubly linked list. Each node stores a reference to a song and pointers to the next and previous nodes in the list.
3. Playlist, which represents a playlist containing multiple songs. It uses a doubly linked list to store the songs. Each playlist has a name and maintains references to the head and tail nodes of the linked list.
4. Jukebox, which represents the digital jukebox with functionalities to manage playlists and playback controls. It maintains a list of playlists and tracks the current playlist index and the current song node being played. It provides methods to add playlists, play/pause songs, skip to the previous or next song, and skip to the first track of the current playlist.

----
To use the digital jukebox:
1. Create songs using the Song class, specifying the title, artist, and duration
2. Create playlists using the Playlist class, giving each playlist a name, and add songs to them using the add_song method
3. Create a jukebox using the Jukebox class and add playlists to it using the add_playlist method
4. Test various jukebox functionalities like play/pause, skipping songs, and skipping to the first track of the current playlist

----
Difficulties encountered:

I struggled with the 'idea' and the 'how' of trying to write and implement tests to see if the code worked properly. I finally decided to do without it and instead include example usage. If I were to include tests, however, I would want to (at minimum):
1. Ensure that the playlists are created correctly with the specified name
2. Ensure that songs are correctly added to the playlist
3. Test for adding multiple songs to the same playlist
4. Check if the head and tail pointers of the playlist's linked list are updated correctly after adding songs
5. Perform checks to ensure the various jukebox functionalities are working
