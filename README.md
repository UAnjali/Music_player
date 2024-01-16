## Music player
## Problem Statement

You love to listen to songs and use Online music streaming applications for listening to music. But as online streaming applications use ads for revenue generation, and you don’t want to listen to those ads. But you like their feature of creating your own playlist and being able to change the playlist content dynamically.

### Goal
Create a Music Player application that enables users to play locally stored songs, as well as create and update playlists with the songs.

### Acceptance Criteria
<ol>
<li>The App must have 4 major sections:
  <ol>
  <li> All songs</li>
  <li>Song card</li>
  <li>Playlist</li>
  <li>Toggle theme</li>
  </ol>
  </li>
<li>The **All Songs** section should render a list of all the songs and should also have the functionality to filter the songs based on genre.</li>
<li>Clicking on any of the songs in the list should play that song.</li>
<li>The **Song card** section should display the song card with the image, name and artist name of the song which is currently played.</li>
<li>It should also include the controls like play, prev and next.</li>
<li>It should also allow the user to add the song to a particular playlist.</li>
<li>The **Playlist** section should display all the playlists already created and an option to create a new playlist.</li>
<li>When a particular playlist is clicked, all the songs added to that playlist should be listed in that section only.</li>
<li>The **Toggle** theme section should be a button which when clicked should change the theme from dark to light and vice-versa.</li>
</ol>

### Tasks
<ol>
<li>Create an array to store all the songs. Each song is represented as an object with id, name, artist, img, genre, and source as its properties.</li>
<li>To change the theme of the app, create a toggleTheme() function, which should set the data-theme attribute to dark or light, depending on its previous value.</li>
<li>For the songs section, create a function showSongs() to render the list of songs depending on the currently selected genre. If no genre is selected, it should render all the songs.</li>
<li>There should be a change event handler for every dropdown menu option, which updates the song list, according to the selected option value, which represents different filters available.</li>
<li>For the Song Card section, the currently selected song should be displayed with its image, song name, and artist name.</li>
<li>It should have control buttons such as “next”, “previous” and “Add to Playlist”.</li>
<li>Create a function renderCurrentSong which could be called whenever a song is selected to render its info in the song card and to play it.</li>
<li>Create a function addtoPlaylist function to handle the click event of the “Add to Playlist” button and add the song to the selected Playlist.</li>
<li>On click of the next button next song should be played, and on click of the previous button, the previous song present should be played. Both the next and previous buttons should be able to handle edge cases.</li>
<li>For the Playlist section, create a function createPlaylist() which should be linked to the click event of the “create playlist” button and should handle creating a new playlist and adding that to all playlist sections.</li>
<li>Create a renderPlaylistSong which should be linked to the click event of all playlists and should beused to display the song present in the playlist.</li>
</ol>

### Additional Tasks
You can add the following functionality to the project to maximize your score:
<ol>
  <li>
    Create a search input field to search for a particular song.
  </li>
  <li>
    Create a search input field to search for a particular playlist.
  </li>
  <li>
    Create an option to remove a song from the playlist.
  </li>
</ol>

### Hints:
The whole project can be divided into 3 div:

-  Heading:  Displays the name of the Music Application and the toggle button.

-   Container:  Displays a form to create and update images in a specific album.
  
The Container can have the following div: 

-    All-song-div:  It can be used to display all the song along with filter option

-    Card div:  It can be used to show the currently playing show along the various control buttons.

-    Playlist div:  It can be used to store all playlists and also the create new playlist option.

## Evaluation Criteria
Your project will be evaluated on the following parameters -
- ALL SONG SECTION  
Render the song correctly using array and implement filter functionalities. (Max Score 15)
- EVENT HANDLING FOR ALL SONG SECTION 
Each song should have onclick event and the filter options should have change event. (Max Score 20)
- SONG CARD SECTION 
The Song details should be rendered correctly, Control Buttons should Function correctly. (Max Score 20)
- TOGGLE BUTTON 
Should be able to change the theme from light to dark and vice versa. (Max Score 15)
- PLAYLIST SECTION 
Should be able to create new Playlist. Newly created playlist should be appended to the all playlist section with the click event. On selecting the playlist the song should be added to that particular playlist. The song added to the playlist should be preserved. (Max Score 20)
- ADDITIONAL TASK 
Should have a search option to search for a song and for playlist. Should have a option to remove a song from playlist. (Max Score 10)
