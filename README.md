![Microsoft Teams](https://developer.microsoft.com/en-us/graph/blogs/wp-content/uploads/2018/11/Teams-Dev-Logo-900x360.png)

osTicket-SimpleWebhook
==============
An plugin for [osTicket](https://osticket.com) which acts as a webhook on new/updated tickets.

Originally forked from: [https://github.com/ipavlovi/osTicket-Microsoft-Teams-plugin](https://github.com/ipavlovi/osTicket-Microsoft-Teams-plugin).

Info
------
This plugin uses CURL and was designed/tested with osTicket-1.14.3

## Requirements
- php_curl
- An API url

## Install
--------
1. Clone this repo or download the zip file and place the contents into your `include/plugins` folder.
2. Now the plugin needs to be enabled & configured, so login to osTicket, select "Admin Panel" then "Manage -> Plugins" you should be seeing the list of currently installed plugins.
3. Click on `SimpleWebhook` and paste your Teams Endpoint URL into the box (MS Teams setup instructions below). 
4. Click `Save Changes`! (If you get an error about curl, you will need to install the Curl module for PHP). 
5. After that, go back to the list of plugins and tick the checkbox next to "MS Teams Notifier" and select the "Enable" button.

## Test!
Create a ticket!

Notes, Replies from Agents and System messages shouldn't appear, usernames are links to the user's page 
in osTicket, the Ticket subject is a link to the ticket, as is the ticket ID. 
