# Music Player
## Backend 
For the backend we used an express web server running the latest version of Node.js. The main backend manager we used was Node.js because it was both versatile and had many 3rd party libraries. 
The Node.js & express server do quite a few things such as…
- Make API calls to gather music data
- Extract the stream URL (from youtube) of a given song
- Provide Album information and artwork  
Any keyword searched is sent to the backend node.js & express server and then subsequently searched on Xiami Music, a Chinese music provider. The downside to this is that some songs are not on Xiami Music due to copyright issues between the producing company and Xiami.
Once the keyword is searched on Xiami and the full album and track info is found, the track info is queried on Youtube. If the user plays the song and a match is found on Youtube, youtube-dl will start extracting a stream url for the song and return it to the user’s phone

## Frontend
The front end design library we used was Material Lite design. Material design is a design philosphy designed by Google and is used throughout their app ecosystem on both Android and iOS. 
So to provide a more consistent user experience on Android we decided to use Material Design Lite which provided us with a simple CSS and JS library to make out app look nice. 
We also used a templating system on the front end which takes in a JSON list and repeats it automatically given and html code.
We used the HTML5 Media API to provide a notification in the system notification tray giving you full media control over the music being played.

## Final Product
The final product had an a fully functional album view page and a search page. 
The search page is also is fully functional providing album art, track title, and album title.

