# 100 Days Of Code - Log

### Day 0: January 28, 2019

**Today's Progress**: 
* Learn Javascript through The Odin Project

**Thoughts:** 
* They redirected me to freeCodeCamp.
* Looks like an old retread. Gonna go back and review on Youtube (where I started).

### Day 1: January 29, 2019

**Today's Progress**:
* Review Javascript [Link](https://www.youtube.com/user/TechGuyWeb)
* Continue learning CSS3 basics [Link](https://www.youtube.com/user/TechGuyWeb)
* Learned Git.
* Learned CSS flexbox, grid, animations, and transitions. 
* Continue doing What2Do app.

**Thoughts:**
* Having trouble integrating javascript files with BottlePy.

**Links**
* [What2Do App](https://github.com/thebinsubtleissubtle/what2do)

### Day 2: January 30, 2019

**Today's Progress**:
* Continue learning Javascript through [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)
* Continued doing What2Do app.
* Continued learning CSS3 Animations and Transitions.
* Learned Spotipy.


**Thoughts:**
* Had 7 commits on this repository because I had trouble with cloning repositories into the local directory.
* Testing animations was fun!
* Installed Ruby + devkit to get SASS.

**Links:**
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)

### Day 3: February 1, 2019

**Today's Progress**:
* Started building TopPlaylist: A web app that tracks the most played songs, albums, artists, and genres. Uses Spotify API and BottlePy. [Inspiration](http://107.170.81.187:8080/)

**Thoughts:**

* Had difficulty implementing Spotify authentication on my web app. 
* Asked the discord community about this issue. I finally cracked the code on Spotify Authentication via this code:

`SP_OAUTH2 = oauth2.SpotifyOAuth(client_id = CLIENT_ID, client_secret = CLIENT_SECRET, redirect_uri = "REDIRECT_URI", scope = SCOPE, cache_path = CACHE)`

**Links:**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle/topPlaylist)
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)


### Day 4: February 3, 2019

**Today's Progress**:
* Continued building TopPlaylist: A web app that tracks the most played songs, albums, artists, and genres. Uses Spotify API and BottlePy. (most_played.html)

**Thoughts:**
* Cleaned code. Instead of passing on placeholder variables, I put it on a single variable.
* Made tables with tracks and artists items. (It's still ugly).

**Links:**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle/topPlaylist)
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)

### Day 5: February 4, 2019

**Today's Progress**:
* Stared re-learning DOM Manipulations.
* Continue building TopPlaylist: A web app that tracks the most played songs, albums, artists, and genres. Uses Spotify API and BottlePy. (most_played.html)

**Thoughts:**
* Began working on modes. (Whether the user wants to show particular types(tracks or artists), terms(short, medium, long), and number of items that will be shown).
* Started working on CSS.

### Day 6: February 5, 2019

**Today's Progress**:
* Learned Parallax website building.
* Continue learning DOM Manipulation.
* Continue building TopPlaylist: A web app that tracks the most played songs, albums, artists, and genres. Uses Spotify API and BottlePy. (Parallax Website, search bar, and landing page.)

**Thoughts:**
* Pushed TopPlaylist on GitHub.
* Started working on search function.
* I made the landing page to a parallax website.
* Had trouble in paging object model when implementing to the web app.

**Links:**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle/topPlaylist)
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)

### Day 7: February 6, 2019

**Today's Progress**:
* Continue building TopPlaylist: A web app that tracks the most played songs, albums, artists, and genres. Uses Spotify API and BottlePy. (Pagination).
* Continue learning DOM Manipulation.

**Thoughts:**
* In search.html, I worked on the functionality of pagination. This was on the previous and next buttons *alone*. It was wrong to load JSON from the link because it's a goddamned link and you can't load json data from an API link. So I made a global variable `LIMIT` and `OFFSET` then made a function `get_offset()` ehich gets the `offset`, `limit`, and `type` that returns a added/subtracted offset value depending on the limit set by user.
* ~~I created another global function called `process_pagination()` which accepts `keyword`, `offset`, `limit`, and `type` values while returning the `result` object.~~ That function is not necessary since it runs the same as `search()`, so I copied it and made it `page()` then `@app.route("/search/<keyword>/<type>")` has now `/<curr_offset:int>/`


**Links:**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle/topPlaylist)
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)

### Day 8: February 7, 2019

**Today's Progress**:
* 

**Thoughts:**

**Links**
