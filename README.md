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
I'm not sure this step is good now. We will be learning more about arrays and hash.

I decide to chenge this step to few smaller to not make big jump.

Music store with only album names... not good. We need add to our data(array) also album songs and change everything to serve this so:

1. add also songs after album( "Add album") with options add songs to existing album
2. remove album with all songs( "Remove Album" )
3. show also songs("Show Albums")
4. add new menu option to remove songs from albums or rebuild second menu option to include submenu with two options... remove album remove song from album

<dl>
  <dt>Hints</dt>
  <dd>to implement this data use nasted arrays/hash(or both mixed)</dd>
  <dd>album should be still uniqe but songs could have the same name differents album</dd>
</dl>


Step three(or it could be also step 4... your choose):
-------------

Please not read if you didn't make second step because you can create chaos in your head;)

Now our music store looks better but good to know albums artists. please implement also artist in our data structure. 

Lets think a little about it. We can add artist to album but better will be add album/albums to artist because one artist can have a lot of albums.
You need make also changes to serve it:

1. add artist before album( "Add album") - if artist exist add to him other album
2. add options to remove artist
3. show also artist ("Show Albums") -capitalize list to show correct structure so show albums option can look:

```ruby
	jackson
		thriler
			song 1
			song 2
			song 3
			...
		bad
			song 1
			...
	MrWhite
		album_one
			song 1
			song 2
			...
```

<dl>
  <dt>Hints</dt>
  <dd>to implement this data use nasted arrays/hash(or both mixed)</dd>
  <dd>artist should be uniqe but albums could have the same name to differen artist but one artist can't have two the same name</dd>
  <dd>if you remove artist you also remove all him albums</dd>
  <dd>album structure should stay not change</dd>
</dl>

Step four:
-------------

if you make this step before step 3 then step 3 will(should) be easier.

good work but it's not look like should. You know conditions, loops, arrays, hashs, iterations, simple methods etc. Nice but this application look like spagetti... all things in one loop. Could you imagine this application if we will have 20-30 options in menu(not 6)? How we can find something and read this code? We can't...

so now is good moment to learn  about class, module, creating methods, declaring methods visibility... please first read about it and think... 

First you can input everything in one class and generate execute method which will be run our program. every options should be in own method.

It's really important point... you need know what it is class, module, method... how working OOP to understand this language