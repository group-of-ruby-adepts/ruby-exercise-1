ruby exercise 1 - Music Store 
===============

We will be learning Ruby on task:
<dl>
  <dt>Target</dt>
  <dd>Create  music album store terminal application in ruby</dd>
  <dt>Teaching way</dt>
  <dd>After any step will be suggestions and refactoring</dd>
  <dt>Suggestions</dt>
  <dd>please don't read next step if you didn't done prev( because it could suggest you something wrong) </dd>
</dl>

Step one:
-------------
You have to create terminal application which after run show:

	What do you want to do? 
	1. Add Album
	2. Remove Album 
	3. Show Albums 
	4. Quit 

* Add Album - get only name  and store it in array
* Remove Album - get album name and remove from array if exist
* Show Albums - print all albums
* Quit  - close app

After any command(except Quit) application should back to this menu. 


Step two:
-------------

Please not read if you didn't make first step.

Great you done part one. You know loops, conditions, sample array, and important/sample methods.
I'm not sure this step is good now. We will be learning more about arrays and hashs.

You have to suggest and implement data structure to our music store(nested hashs and arrays). New menu will be hint also:

	What do you want to do? 
	1. Add Artist
	2. Add Album to Artist
	3. Remove Artist(with all albums)
	4. Remove Album
	5. Show Artists
	6. Show Albums
	7. Serach Artist by music kind
	8. Search songs
	9. Quit 

* 5. Show Artists - example:
	MrWhite(Rap)
		albums:
			"hard album" - 2 songs
			"street child" -3 songs
	Metalica(Metal)
		albums:
			"Inferno" -2 songs

* 6. Show Albums - example:
	hard album:
		first song
		second song
	street child:
		coke and casino
		trouble with programming
		tabasko
	inferno:
		hard song
		mega hard song
		
* 7. Serach Artist by music type
	Please write music type?
	Rap # input Rap
	MrWhite(Rap)
		albums:
			"hard album" - 2 songs
			"street child" -3 songs
	
* 8. Write song name(or part)
	song #type song	
	Find songs:
		first song(hard album - MrWhite)
		second song(hard album - MrWhite)
		hard song(inferno - Metalica)
		mega hard song(inferno - Metalica)

	
<dl>
  <dt>Hints</dt>
  <dd>Artist have be uniq</dd>
  <dd>artist have music type not album</dd>
  <dd>point 4 can remove more then one albums if have the same name</dd>
</dl>

Step three:
-------------
