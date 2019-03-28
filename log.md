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
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)


### Day 4: February 3, 2019

**Today's Progress**:
* Continued building TopPlaylist: A web app that tracks the most played songs, albums, artists, and genres. Uses Spotify API and BottlePy. (most_played.html)

**Thoughts:**
* Cleaned code. Instead of passing on placeholder variables, I put it on a single variable.
* Made tables with tracks and artists items. (It's still ugly).

**Links:**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)
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
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)

### Day 7: February 6, 2019

**Today's Progress**:
* Continue building TopPlaylist: A web app that tracks the most played songs, albums, artists, and genres. Uses Spotify API and BottlePy. (Pagination).
* Continue learning DOM Manipulation.

**Thoughts:**
* In search.html, I worked on the functionality of pagination. This was on the previous and next buttons *alone*. It was wrong to load JSON from the link because it's a goddamned link and you can't load json data from an API link. So I made a global variable `LIMIT` and `OFFSET` then made a function `get_offset()` ehich gets the `offset`, `limit`, and `type` that returns a added/subtracted offset value depending on the limit set by user.
* ~~I created another global function called `process_pagination()` which accepts `keyword`, `offset`, `limit`, and `type` values while returning the `result` object.~~ That function is not necessary since it runs the same as `search()`, so I copied it and made it `page()` then `@app.route("/search/<keyword>/<type>")` has now `/<curr_offset:int>/`


**Links:**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)
* [Traversy Media (youtube)](https://www.youtube.com/user/TechGuyWeb)

### Day 8: February 7, 2019

**Today's Progress**:
* I made the filtering list on `search.html` and made `most_played.js`

**Thoughts:**
* I made `most_played.js` due to a fact that if I combined the scripts from `index.html` and `most_played.html`, the scripts won't work properly. 
* On `most-played.js`, I made a client-side filtering to make sure that the whole page doesn't reload after submitting the form. I used the `e.preventDefault()` to prevent the form from posting the data. The filtering is good. I want to do some animations later on.
* On `main.py`, I just put `@app.route("/most_played/", method = "POST")` because there is a form. But if I didn't do that, it returns an error 405 page.
* I just hide the tables in `style.css`. Hiding it on-load is a pain in the ass.

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 9: February 8, 2019

**Today's Progress**:
* I fixed the search navigation buttons and added a `search.js` to integrate with `search.html`
* I made the `get_offset_data()` in `main.py` to be passed to `search.js` via a hidden paragraph in  `search.html`

**Thoughts:**
* I can't figure out how to pass JSON data as a parameter to a Javascript file, so I made the hidden field to `search.html` then parse it to JSON because the `offset_data` that I put in `#offset-data` is a raw text.

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 10: February 9, 2019

**Today's Progress**:
* I continued the CSS on `search.html` 
 
**Thoughts:**
* I added transitions on `index.html` search bar.
* I put borders first on every wrapper. I wrapped every part of search results using `.track-results-wrapper`, `.artist-results-wrapper`, `.album-results-wrapper`. And then I wrapped every query using `.track-result`, then I wrapped every element. It's just the `track` element.

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 11: February 10, 2019

**Today's Progress**:
* Added some animations on `search.html`
* Fixed the default value of `#search-type`. I added the `get_type` variable, which is a dictionary (`dict()`) that gets the `type` and turns it into a JSON variable. Once it passed to the template and put in a hidden `<p>`, the `search.js` processes the JSON variable passed by the template, and changes the value of the default value of the select form `#search-type`.
* Started working the CSS of `most_played.html`

**Thoughts:**
* I always had trouble on getting `spotify.client.SpotifyException`. It says that `The access token is expired`, so it always throws an error (`unauthorized url` and `spotipy.client.SpotifyException`). But when I reset the server, the error is gone. 
* While I'm fixing the `search(keyword, type)` function, looping it and passing `None` to `type`. And when the `spotipy.client.SpotifyException` is thrown, the `NameError` is thrown too. I'm still trying to solve this though. 

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 12: February 11, 2019

**Today's Progress**:
* Started learning Flask through ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* I though BottlePy and Flask the same because they are both web microframeworks, then I realized Flask has extensions like form validations (flask-wtf), Jinja templating (I mean *Jinja Templating*), bootstrap (flask-bootstrap), and moment.js, which is a Javascript tool for getting the current time and date. Going back to Jinja templating, it is very easy to work with, instead of repeating every *goddamn boilerplate HTML*. It makes life easier by using `{% block %}`. Then I realized, my [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist) has a lot of boilerplate code. I'll save that for future projects from now on.
* I got a job interview tomorrow, does it break my streak? Doing something like 3 hours/day? Damn I'm not ready yet.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 13: February 13, 2019

**Today's Progress**:
* On chapters 5 & 6 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* I learned how to set up the database first by SQLite. It was hard at first, considering that I have little knowledge about SQLite. Then I got into trouble when querying the user roles using `user_role.users.order_by(User.username).all()`. When I added `lazy = "dynamic"` into my `Role.users`, the query returns `AttributeError: 'InstrumentedList' object has no attribute 'all'`. Then when I restarted the IDLE, it works!
* An error spotted when I send email everytime the system detects a new user, then I realized that I typed `sneder` instead of `sender`

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 14: February 14, 2019

**Today's Progress**:
* Made Spotify login status.
* Changed footers on all pages.
* Added "`No preview available`" on `search.html` 

**Thoughts:**
* I added the `global LOGIN_STATUS` on every route function because the `LOGIN_STATUS` value changes when the app redirects to another page. For example, if I go to `/verified`, the `LOGIN_STATUS` sets to `True`, but when it redirects to `/most_played`, the value changes to `False`, its default value.
* I added the `#most-played-body` on `most_played.html`, because if I changed the background of the body to `#292823`, every page will be affected by this change.. I still can't send the footer to the bottom page of the screen, damn you footer. 

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 15: February 16, 2019

**Today's Progress**:
* Made some animations on `most_played.html`.
* Learned Julia Language

**Thoughts:**
* I still can't figure out how to put the footer into the bottom of my screen. If the footer was `fixed`, the footer will stick to the bottom of the screen no matter what. If I set the footer to `absolute`, the footer will adjust to the bottom of the screen when the results shows, but it does not adjust when they are not.
* I wrapped the images on a `<td>` so the texts will not go after the images.
* Julia Language is easy to pick-up language. I haven't encountered `macros` throughout my programming career. It's more Pythonic except it does not focus on general OOP concepts.

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)
* [Tutorial](https://www.github.com/thebinsubtleissubtle2/julia-tutorial)

### Day 16: February 17, 2019

**Today's Progress**:
* Removed `#about` div in `index.html`
* Started working on making playlists.

**Thoughts:**
* I encountered an error that is concerned with making playlist. `spotipy.client.SpotifyException: http status: 400, code:-1 - https://api.spotify.com/v1/users/iamnomusicenthusiast/playlists:` I can't make a damn playlist on my REPL code, even though it was copy-pasted from [here](https://github.com/plamere/spotipy/blob/master/examples/create_playlist.py).
* I have problems styling the `.modal-footer`, having the `background-color` same as `.modal-header`. The close button comes first before the create playlist button.

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 17: February 19, 2019

**Today's Progress**:
* Made the sessions through `beaker.middleware`

**Thoughts:**
* At first, I still can't figure out how sessions work in BottlePy since it has no configurations on sessions. I thought sessions are safer than cookies, because the user data put in the forms are unsafe, because it is personal data. So, I figured out how to deal with sessions using Beaker. I tried the sample codes in Stack Overflow. I ended up with `request.session["logged_in"]` instead of putting `request.environ.get("logged_in")` to every route function. I also put this code below before the static files. 

`@hook("before_request")
def setup_request():
	request.session = request.environ["beaker.session"]`

Now I am going to work on dropdown menu bar and continue working on playlists. 

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 18: February 20, 2019

**Today's Progress**:
* No commits today.

**Thoughts:**
* The reason that I can't make playlists on Spotify via their API is that what I used ([Spotipy](https://github.com/plamere/spotipy)) **was freaking outdated on [PyPi](https://pypi.org/project/spotipy/).** So, I uninstalled the package using `pip uninstall`, and re-installed it using the [source code](https://github.com/plamere/spotipy). Now I have to rewrite the whole program because it returns an error saying:

`requests.exceptions.HTTPError: 401 Client Error: Unauthorized for url: https://api.spotify.com/v1/me/`
`spotipy.client.SpotifyException: http status: 401, code:-1 - https://api.spotify.com/v1/me/:`

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 19: February 21, 2019

**Today's Progress**:
* Implementing the creation of playlists.

**Thoughts:**
* The create playlist feature finally worked! Then when I added the tracks, the program returns an error again, and I can't add tracks to playlists. So I created the `list()` variable, because the `user_playlist_top_tracks` accepts the list of `ID`s from the tracks. For each track in the `current_user_top_tracks()` variable, I add the track ID to the `list` variable.
* On implementation, I've encountered yet another problem, styling the button that opens the modal. So, instead of the modal being in the `#search-field`, I put it on every track results before the `table` wrapper. And the modals doesn't show when I'm on `medium term` and `long term` `tracks`.

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 20: February 23, 2019

**Today's Progress**:
* Creating playlists is successfully implemented!

**Thoughts:**
* I refactored the `filterList()` code in `most_played.js`, then I added some functionality on opening the modal by adding a hidden input named `playlist_term`, which contains the value of `term`. I also updated the option values of `term` to `short_term`, `medium_term`, and `long_term` to match the values of parameter `time_range` in `spotify_current_user_top_tracks()` function. 

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

### Day 21: February 24, 2019

**Today's Progress**:
* Continued ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* I haven't worked on learning Flask yet, and at the time I am on chapter 6. I am on chapter 8, and had trouble on running `flask test`, which the program showed an error that says `ERROR: No such command as 'test'`. Then when I checked on my copy of `flasky` that I had just cloned from [here](https://www.github.com/miguelgrinberg/flasky), and found out that my `email.py` and my `forms.py` was empty.
* I also had a trouble dealing with password hashing. When I ran `flask shell`, then I ran `u = User()`, an error appeared as `NameError` which points the `User()`. I came up with the solution, with `from app.models import User`. 
* I might not go through the [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist), although I might work on recommendations feature, and might focus on front-end programming for myself.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 22: February 25, 2019

**Today's Progress**:
* Continued ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com) 

**Thoughts:**
* I am currently working on this error `TypeError: '<' not supported between instances of 'str' and 'int'` that is bothering on my program. I'm still on chapter 8, on creating login forms.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 23: February 26, 2019

**Today's Progress**:
* Still on chapter 8 on ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* Shit. I took another exam, eh? It's on front-end anyways. I walked out because 1) I never liked waiting for another 2 hours and 2) I need to finish this Flask book. 
* I encountered a problem in which my program doesn't log in and returns a blank page. I tried to comment this piece of code that links to my homepage.
`next = request.args.get('next')
 if next is None or not next.startswith('/'):
    next = url_for('main.index')`
Then nothing happened. I tried to google this problem, then I went [here](https://github.com/miguelgrinberg/flasky/commit/80da3d33e64a998bfc3481d3e63a0d04ae5364b1), then I forgot to put `UserMixin` on `class User(UserMixin, db.Model):` on `app/models.py`.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 24: March 1, 2019

**Today's Progress**:
* Having trouble with user registration (["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)).

**Thoughts:**
* New day, new problem. When I click the register button on my registration form in `app/templates/register.html`, my program returns a blank page. I can't see the error here besides `TypeError: '<' not supported between instances of 'str' and 'int'`. It should send the confirmation email to the email address the user has given. 

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 25: March 2, 2019

**Today's Progress**:
* Finished chapter 8 of (["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)).
* Did some [codewars](https://www.codewars.com)

**Thoughts:**
* Yesterday I've received an email for an interview. I made the(ir) cut! I did some Java and (more) Python on Codewars. I solved some problems including the CamelCase method problem. I did that in `Python`, and here's what I've came up:
`def camel_case(string):
    if string == "":
        return string
    arr = string.split(" ")
    for k, v in enumerate(arr):
        if v == "":
            arr.pop(k)
        arr[k - 1] = arr[k - 1].capitalize()
    return "".join(arr)`

    More [here](https://www.codewars.com/users/thebinsubtleissubtle/completed_solutions).

* On Flask tutorial, I only did copy the book's source code, because the program returns an `smtplib` error everytime I send the confirmation email to the email address the user has provided.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)
* [Codewars](https://www.codewars.com/users/thebinsubtleissubtle)


### Day 26: March 3, 2019

**Today's Progress**:
* Finished chapter 9 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* Not really much here. I'm on chapter 10 of this book, on the user's profile part. What I learned here is giving user's role to this website. The administrator can do really much everything, moderator moderates posts and comments. It's getting like reddit anyways, without the up/down vote system.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 27: March 4, 2019

**Today's Progress**:
* On chapter 11 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* I thought the package `Faker` is only on Rails. Anyways, I've encountered an error midway through pagination, where I just forgot the `.` in `url_for('.user', username=post.author.username)`, and the `_macros.html`, where I typed `url_for(endpoint, page=pagination.page - 1, **kwargs)` instead of `url_for(endpoint, page=pagination.prev_num, **kwargs)`, my `{% endif %}` was placed before the `{% else %}`, and I've put the `class="diaabled"` (shit I'm a web developer now, I can't spell correctly on my keyboard). Submitting posts was still non-functional, as well as the search function, I believe. I might discover how to do that in this book.
* Damn, interview tomorrow, just damn. ***I hate capitalism***.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 28: March 6, 2019

**Today's Progress**:
* Continued chapter 11 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* One day ago, I said that submitting posts is non-functional. I thought this was actually non-functional, but then I realized, it was an error on my part. I checked the original source code and compared it to mine. I found out that instead of `post = Post(body=form.body.data, author=current_user._get_current_object())`, my program's version has `post = Post(body=form.post.data, author=current_user._get_current_object())`, and I have found out that I put `body` instead of `post` in `app/models.py`. I only finished chapter 11 for today.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 29: March 7, 2019

**Today's Progress**:
* On chapter 12 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* Having troubles on implementing followers on the users page. When I click the followers/following button, it returns to empty page, and the user followers doesn't increase once I hit the follow button. 

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 30: March 8, 2019

**Today's Progress**:
* On chapter 13 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* I got the error! I successfully implemented the followers feature! I mistyped again on `app/templates/followers.html`. Instead of `{% block title %}Flasky - {{ title }} {{ user.username }}{% endblock %}`, I put `{% block title %}Flasky - {{ title }} {{ user.username }}{% enddblock %}` on the title page. I'm on chapter 13 now. Did I said it would look like reddit without the upvotes/downvotes? It looks like it!
* Shit. I've come this far, then I just recently installed Dota 2 on my laptop. 

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 31: March 9, 2019

**Today's Progress**:
* On chapter 14 of ["Flask Web Development by Miguel Grinberg"](https://flaskbook.com)

**Thoughts:**
* I finished chapter 13 of this book. I figured out how to moderate user comments by just closing the comment section. It's just like closing an issue in Github. Now I am going to learn how to build a RESTful API using flask. 
* My thoughts are getting shorter and shorter on my journal as my Flask project progresses. I might go again to [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist) since it is dusted for 3 weeks now. I haven't touched anything on this project since I continued on my tutorials. I might play around APIs again on my next Flask project. Maybe how to improve on Dota 2 I think? Or maybe get something from [here](https://github.com/toddmotto/public-apis).

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 32: March 11, 2019

**Today's Progress**:
* Still on chapter 14 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* Had only a few today. I only managed to implement token-based authentication and by going to `http://localhost:5000/api/v1/tokens/`, finally I have to see my token in my browser.
* I played 3 games today (2 of them are ranked). All of them lost. What the hell?

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 33: March 12, 2019

**Today's Progress**:
* Still on chapter 14 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* I am really, really sorry, but it's short again. I am having trouble earlier implementing the resource endpoints on `api/posts.py`, then when I ran the server, the browser returns a blank page. It is solved now because my `api/users.py` doesn't exist.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 34: March 13, 2019

**Today's Progress**:
* Finished chapter 14 of ["Flask Web Development" by Miguel Grinberg](https://flaskbook.com)

**Thoughts:**
* I finally implemented the API module of this book. I tested modules using `httpie`, I posted blog posts, comment to blog posts, navigate the user's timeline using CLI commands of `http --json --auth <email>:<password> <GET|POST|PUT> http://127.0.0.1:5000/api/v1/<endpoint>`. I can implement this on any websites/projects and get the content of all posts and user's content through the program's API. I understand now how API works. 

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 35: March 15, 2019

**Today's Progress**:
* On chapter 15 of ["Flask Web Development"](https://flaskbook.com)

**Thoughts:**
* I learned from this chapter that writing test scripts on the client side is more efficient than testing it out manually through the server. I've encountered an error earlier on `tests/test_client.py`. I tried using `self.app.testing = True`, but it didn't work. Then I found out that instead of `def setUp(self)`, I mistyped again to `def setup(self)`. What is wrong with this? Should it really be `setup`?

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 36: March 16, 2019

**Today's Progress**:
* Finished chapter 15 of ["Flask Web Development"](https://flaskbook.com)

**Thoughts:**
* This book suggests testing on Chrome, so I installed the chrome driver. And my chrome updated to Chrome 73, so I installed Chrome Driver for Chrome 73. Now I learned that without opening the browser manually, my test scripts automatically tests all of the moduels, including the admin page, and anonymous user. 

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 37: March 20, 2019

**Today's Progress**:
* Finished chapter 16 of ["Flask Web Development"](https://flaskbook.com)

**Thoughts:**
* My source code returns blank page again. I don't understand why it keeps on displaying blank pages on blueprints. So, for the second time, I copy-pasted the source code from github to mine, and migrated the database. I'll say it's harder to debug on blueprints because it always returns `TypeError: '<' not supported between instances of 'str' and 'int'` and blank page on my browser. Even though the original says `@main.after_app_request` and `@main.route('/shutdown')` decorator should be on top, it does not work.
* I just finished chapter 16 of this book. It's on performance and profiling. I had registered my Heroku account because the next chapter will focus on deployment.

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)

### Day 38: March 21, 2019

**Today's Progress**:
* On chapter 17 of ["Flask Web Development"](https://flaskbook.com)

**Thoughts:**
* Had problems earlier accessing my deployed app to heroku. It always shows `application error` whenever it loads. I deleted and recreated the app in my client, but it doesn't work. Then I realized I didn't include the `Procfile`. So I pushed it to my heroku `.git` (`git push heroku master`), then deployed it again using `heroku run flask deploy`. My website crashed! It is [here](nooblog.herokuapp.com). I'm already finding alternatives to heroku because I ran a lot of problems. Maybe Github pages?


**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)


### Day 39: March 22, 2019

**Today's Progress**:
* Still on chapter 17 of ["Flask Web Development"](https://flaskbook.com)

**Thoughts:**
* I solved my Heroku problems, but run on another problem on Docker. I figured out the problem on heroku and my Flask, and Werkzeug versions are not the latest, so I changed it to `Flask==1.0.2` and `Werkzeug==0.14.1`.
* Now on the Docker problem, I can't run my application. It says `docker: Error response from daemon: container 4845a609c92d05abf9aa15b97817b3e3a57fcbf9b6e79f086a96f5f2822bc33f encountered an error during CreateProcess: failure in a Windows system call: Unspecified error (0x80004005)`. I googled this and I found different problems like `No hypervisor is present on this system`, or `The handle is invalid. (0x6)`. I switched my containers to Linux, no avail, it says `Not enough memory space to run`.

* The Nooblog website is [online](https://nooblog.herokuapp.com)!

**Links**
* [Flask Tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial)
* [Nooblog](https://nooblog.herokuapp.com)

### Day 40: March 26, 2019

**Today's Progress**:
* Started rewriting [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist) in Flask.

**Thoughts:**
* Yeah boys. Back to developing topPlaylist again. I am working on Flask's version of this project, and so far it was really different from the previous one. For the old one, I'm currently working on recommendations. For the new ones, I am making cleaner by applying concepts that I learned from my [Flask tutorial](https://www.github.com/thebinsubtleissubtle2/flask_tutorial).

**Links**
* [TopPlaylist2](https://www.github.com/thebinsubtleissubtle2/topPlaylist2)

### Day 41: March 28, 2019

**Today's Progress**:
* Started working on recommendations.

**Thoughts:**
* I made a REPL code for my recommendations feature on Spotipy. I gathered all the URLs from the top tracks, artists, and put them into separate lists. I also called `recommendation_genre_seeds()` function to get all the genres provided by Spotify. Then the results are `warning:expected id of type %s but found type %s %s` and `requests.exceptions.HTTPError: 414 Client Error: Request-URI Too Long for url`. It's in the docs guys, why not update the docs?

**Links**
* [TopPlaylist](https://www.github.com/thebinsubtleissubtle2/topPlaylist)

