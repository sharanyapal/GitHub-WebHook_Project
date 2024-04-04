# GitHub Webhook Receiver
Create a GitHub repository to automate sending webhook events for specific GitHub actions (Push, Pull Request, Merge) to a registered endpoint. The endpoint should store these events in MongoDB. The UI should periodically fetch data from MongoDB and display the latest changes from the repository.

> Implementation Guidelines:
  ~ Utilize GitHub webhooks for integration with the action repository.
  ~ Develop the endpoint using Flask, following provided base code.
  ~ Store data in MongoDB with specified schema.
  ~ Design a clean and minimal UI, fetching and displaying data every 15 seconds.

> Submission Details:
  ~ Set up two repositories: action-repo for GitHub actions with webhooks, and webhook-repo for the endpoint.
  ~ Customize provided base code to meet task requirements.

> Sample UI Output Format: Keeps polling from a given repo and updates itself after every 15 seconds.

  ~ PUSH Action:
      {author} pushed to {to_branch} on {timestamp}
      Sample: "Travis" pushed to "staging" on 1st April 2021 - 9:30 PM UTC
  ~ PULL_REQUEST Action:
      {author} submitted a pull request from {from_branch} to {to_branch} on {timestamp}
      Sample: "Travis" submitted a pull request from "staging" to "master" on 1st April 2021 - 9:00 AM UTC
  ~ MERGE Action (Bonus):
      {author} merged branch {from_branch} to {to_branch} on {timestamp}
      Sample: "Travis" merged branch "dev" to "master" on 2nd April 2021 - 12:00 PM UTC

> Tools and Languages Used:
1. Designing: Basic HTML, CSS (with Bootstrap 5)
2. Frontend: JS
3. API: FetchAPI, JQuery
4. Microframework: Flask
4. Databases: MongoDB.
5. Server:: Flask Default Server.
Merge (Bonus): {author} merged branch {from_branch} to {to_branch} on {timestamp}
