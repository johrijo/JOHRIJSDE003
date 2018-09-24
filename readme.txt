INTRODUCTION:
I used graph api to get the Facebook feed of my account using javascript Facebook library. 

NOTE: 
Original request was to get the feeds from Expedia's Facebook page but Facebook requires a APP review process to read from public pages, hence i couldn’t achieve it. Instead this Code retrieves feed from one's own Facebook account.
Facebook App Review process :  https://developers.facebook.com/docs/apps/review/

Login code is based on Facebook Login Example.

SOLUTION EXPLANATION
1. Using FB javascript library, i make a call to FB.getAuthResponse() that gives me if i'm logged in or not. If I’m logged in, i get the access Token.
2. With the access token i call the '/me' api. 
3. The api returns the json data, which I display in a tabluar format. -- i use javascript DOM api to create the table. 

HOW TO EXECUTE THIS

1. Create a new facebook app in https://developers.facebook.com/apps/ and update the app id in the index.html (line 93)
2. Open https://johrijo.github.io/JOHRIJSDE003/ and this will display the UI for extracting one's own Facebook feed.
3. Click on the facebook login button. This will attempt to login into the page. 
4. A message will be displayed "Thanks for logging in, <Your name>!"
5. After that click on "Get your Feeds"
NOTE: Currently it will not alow other users to fetch  as the Facebook APP review is not Done (https://developers.facebook.com/docs/facebook-login/permissions#reference-user_posts)
(let me knmow if you want to be a developer/tester of my app, i'll send you a requrst and you can retrieve your posts )
6. A table of your last 10 feeds feed will be displayed

DEMO VIDEO
demo and code walkthrough : Q3 Demo Video.mp4

