# RSS Reader with Reminder

**This sample requires redis**. Make sure to run FLUSHALL in redis-cli between samples.

This is a simple RSS reader that uses two storage, one for storing a feed source and another for storing feed results. You can keep refreshing your browser and the RSS Reader will display the latest results whenever they are available.

- Make sure you have redis installed and running.
- Run the app using `dotnet run`.
- Open `localhost:5000`
- You can keep refreshing the browser page as much as you want and it will only pick up and store unique feed items.
- Orleans will keep keep refreshing each feed every x minutes (configurable). 