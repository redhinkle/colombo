# colombo
Colombo episode grabber with YouTube API


For this final I chose to make an API call to YouTube to fetch data of a certain category of videos (in this case, episodes of 'Colombo').

I utilized the Google API website to create an API key for myself and grab data from the channel. The data can be seen here.

With this data I created a component called VideoList which would break up 3 variables from the Google API URL: the id of the YouTube channel, my API key, and the number of videos to display. I then created a new variable called 'URL' that held the original URL but this time injected the three new variables so they are interchangeable in case I want to change which channel I pull from.

Inside the VideoList component I included a state object that carried 3 property arrays: videos, titles, and desc. These are initially empty arrays however when the component is mounted with the componentDidMount() function they are populated with those values from the fetched data with their respective values.

The VideoList component then will render a map of the state arrays so each iteration will return a div that contains the title, YouTube iframe, and description.

-Jared Hinkle 2020
