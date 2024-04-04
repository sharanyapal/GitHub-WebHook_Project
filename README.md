Create a GitHub repository to automate sending webhook events for specific GitHub actions (Push, Pull Request, Merge) to a registered endpoint. The endpoint should store these events in MongoDB. The UI should periodically fetch data from MongoDB and display the latest changes from the repository.

# Implementation Guidelines:
<br> ~ Utilize GitHub webhooks for integration with the action repository.</b>
<br> ~ Develop the endpoint using Flask, following provided base code.</b>
<br> ~ Store data in MongoDB with specified schema.</b>
<br> ~ Design a clean and minimal UI, fetching and displaying data every 15 seconds.</b>

  </b>PUSH Action:</b>
   <br> ~ {author} pushed to {to_branch} on {timestamp}</br>
   <br> ~ Sample: "Travis" pushed to "staging" on 1st April 2021 - 9:30 PM UTC</br>
  </b>PULL_REQUEST Action:</b>
   <br> ~ {author} submitted a pull request from {from_branch} to {to_branch} on {timestamp}</br>
   <br> ~ Sample: "Travis" submitted a pull request from "staging" to "master" on 1st April 2021 - 9:00 AM UTC</br>
  </b>MERGE Action (Bonus):</b>
   <br> ~ {author} merged branch {from_branch} to {to_branch} on {timestamp}</br>
   <br> ~ Sample: "Travis" merged branch "dev" to "master" on 2nd April 2021 - 12:00 PM UTC</br>
 
<b>Tools and Languages used:</b>
<br>1. <b>Designing:</b> Basic HTML, CSS (with Bootstrap 5)
<br>2. <b>Frontend:</b> JS
<br>3. <b>API:</b> FetchAPI, JQuery
<br>4. <b>Microframework:</b> Flask
<br>4. <b>Databases:</b> MongoDB.
<br>5. <b>Server:</b>: Flask Default Server.
