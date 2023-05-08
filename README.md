Download Link: https://assignmentchef.com/product/solved-radio-station-management-system
<br>
WKRP, the local radio station wants to computerize the creation of its playlists. Playlists are the lists of items that will be broadcast in a set period of time. A data file exists containing items that can be part of a playlist. Some entries are songs: a category of song, song’s title, artist/group, play time and audio file. Other entries are commercials: category, company, play time and audio file. Other entries are ‘talk shows’ : category, title, host, play time and audio file. All items have a unique item id.

The radio station wants an interactive application that will do the following:

Allow the disc jockey to add a talk show, song or commercial to the library

–     the user should be prompted initially for the id number. If the id has already been used the user should be told the id is already in use and prompted for another id value. Once the id is valid the user is allowed to enter the appropriate information for the item (e.g. if it is a song, the user should be prompted for title, artist/group, play time and audio file)

Allow the disc jockey to delete a talk show, song or commercial from the library using the id.

–     the user should be prompted then allowed to enter the id number of the item to be deleted

Allows the disc jockey to print the complete list of items in the data base or allow the disc jockey to print the list for all items of a particular type (i.e. song, commercial or talk show)

–     the user, should then be prompted for the category of item being searched for (i.e. classical (L), country (C), rock (R), pop (P), and alternative (A)), then the list of items should be returned and displayed on the console.

produce a play list showing a random selection of talk shows, songs and commercials for a time segment – the time of the segment to be input by the disc jockey.

<strong>Details:</strong>

The talk show categories are: science (S), politics (P) and miscellaneous (M)

An example of a record in the talk show data file is shown below.

e.g.      1001,S,The Newest Planet, Dr. Jones, 53:30, planet.mp3

The song categories are: classical (L), country (C), rock (R), pop (P), and alternative (A). An example of a record in the song data file is shown below:

e.g.      1003,P, Rain Down On Me, Blue Rodeo, 4:49, BR2.mp3

The commercial categories are: vehicle dealers (V), household products (H), computers (C), and miscellaneous (M).

An example of a commercial track would be

1008,C,Computers ‘4 Less, 0:30, comp4less1.mp3

<strong>Assignment:</strong>

Given the details for the Song, Commercial, and TalkShow classes for this assignment:

List the attributes that TalkShow, Song and Commercial have in common and create an Item class based on these common attributes

Create the TalkShow class, the Song class and the Commercial class so that they extend the Item class.

Add constructors and a toString() and equals method to each class using super where necessary.

Create an application to implement the functionality described above. The application should be controlled by a menu with selection choices to Add, Delete and Query the items, create a Random Playlist and exit program. You will need the following operational methods in your application.

Create a method to fill a ArrayList with items. (These items could be talk shows, songs or commercials.) There should be a private validate method to check that each item being created is valid – i.e. each has a valid type that matches a valid id number.

Item id            ends with       0-2      Talk show

Item id            ends with       3-7      Song

Item id            ends with       8-9      Commercial

Create a method that prints the contents of the list by accessing a toString method from each of the item classes. Use an iterator to do this.

In addition to the above method create a search method that prompts for the category (i.e. song, commercial or talk show) and then prompts for the sub category for songs, commercials, or talk shows mention earlier in the documentation and prints the search results to the console.

Create a <strong>private support method</strong> that will search the list by id and return the item if found or null if not found.

Create a method to add an item if it does not already exist in the list. Use your search method that you developed in <strong>(d)</strong> above.

Create a method to delete an item if it exists. Use your search method.

Create a method to return a random play list given a fixed time in minutes (+ or – 30 seconds).

The program should write the current updated list of items in memory back to the text file when the program exits.

Create a method that controls the menu and contains the 6 selections listed below:

Add a new Song, Talk Show or Commercial

Search for a item by id

Remove a Song, Talk Show or Commercial by id

Create a random playlist given the amount of time

Print complete list or items by category

Exit the program.