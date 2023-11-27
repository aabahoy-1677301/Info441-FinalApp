# Info441-FinalApp

Project Description
As the dissemination of music, particularly over the internet, has evolved so has the desire to
discuss music. Apps like Spotify have already tried to incorporate features that promote this
discussion with their year end lists and stats. However, only being able to discuss and compare
music once a year is not enough for many music listeners. Much of them have moved to
platforms such as tik tok or youtube that allows users to make short video making lists and
making comparisons. But still, not everyone is a content creator in that sense. There are a
plethora of users who would rather just make these fun comparisons to discuss and talk with
their friends. Because of this we wanted to make a website that allows these users to interact
with friends in further music discussion. As a developer and more importantly a music fan, this
necessity for further discussion is enough. Especially when the current outlets for this music
quiz discussions either don’t have the functionality to share and discuss with other users or
aren’t geared towards the kinds of people that would promote these platforms. Therefore limiting
the popularity of these platforms, which we will fix.
Technical Description
Architectural Diagram
Flow Chart
User Stories
Priority User Description Technical Implementation
P0 As a user, I want to compare my musical knowledge
with other users through a live quiz where you
guess the song based on song snippets organized
by genre.
Build a real-time testing
front-end with HTML, CSS,
and Express.js. Utilize
MongoDB for the live player
score and the song data to
store the songs that have
showed up in the tests. Utilize
the Spotify API to retrieve
the song snippets. Host
website on Azure using the
Axios library.
P0 As a user, I want to be able to create an account
and login to access past test data and organize my
profile.
Utilize Auth2.0 for
token-based authorization
that leverages existing
Spotify account.
P1 As a user, I want to export the songs that I just took
a test about into its own separate playlist.
Create a CSV file for all the
song data, and leverage the
Spotify API to transform the
CSV into an actual Spotify
playlist.
P2 As a user, I want to listen to the songs that have
appeared on tests before.
Use MongoDB to store the
songs that have appeared in
tests. Utilize Spotify API to
show widget that allows the
playing of music.
Endpoints
GET /music/{song}/snippet - will play song snippet to the user
GET /music/{song}/details - is the correct answer to the snippet played
GET /user/{id} - user profile details
GET /user/{id}/score - shows users their previous scores
POST /user/{id}/profile - stores user profile in database
POST /user/{id}/score - stores user’s most recent score
