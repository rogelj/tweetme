Watson Personality Insights with Twitter
-----------------------------------
This is an example of a web-based application for analyzing a Twitter user's timeline of tweets with Watson Personality Insights.
The app can be paired with a Twitter bot to create a fun user interaction.

To get the web app running:
1. Create an instance of the Watson Personality Insights service on Bluemix called tweetmewatson-PersonalityInsights.
2. Add a Twitter app on [Twitter](https://apps.twitter.com/) and update the credentials in app.js.
3. Fork this project and give your new app a unique name.
4. Update the manifest.yml file host and name credentials to match your app name.
5. Deploy using workspace content.

This code acts as an example of the updates needed to get an NPM available to nodes in Node-RED.  You can fork the code and deploy or create a new app from scratch and edit it in DevOps Services/GIT

To get the Twitter bot running:
1. Deploy the Node-RED Starter.
2. Bind the Watson Personality Insights Service you already created to your application in Bluemix.
3. Add GIT.
4. Update package.json and bluemix-settings.js.
5. Import the flow in Node-RED from /nodered/tweetmewatsonflow.txt.
6. Update the credentials in "Get Tweets for Insights" function node with the credentials for the Twitter app you created in Step 2 of the web app.
7. Open the Tweet Body node and update "http://tweetmewatson.mybluemix.net?user={{handle}}" and replace tweetmewatson with your app name. 
8. Deploy and Tweet!
