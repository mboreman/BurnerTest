# Echobot

![alt text][logo]

Echobot is a simple starter app for the Burner Developer Connection that shows you how to a how to build a simple bot and add it to a Burner line.

### Prerequisites

* [Burner account + at least one Burner number](https://www.burnerapp.com)
* [Heroku account](https://www.heroku.com) (free)

### Tutorial

1) On your Burner account, enable the Developer Connection from the [Developer Console](https://app.burnerapp.com/developer).

2) Generate an incoming webhook

3) Deploy the Echobot to your Heroku account by tapping the button below. This will install echobot as an app running on your heroku account.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

4) When prompted, enter the Copy and paste the incoming webhook url that was generated above into the "incomingwebhookurl" field of the Heroku form.

![alt text][incoming]

5) Tap "Manage" after echobot has finished deploying to heroku.

![alt text][manage]

5) Find your heroku url under Settings->Domains and paste it into the Outgoing webhook field on the Burner developer console with `/listen` appended to it. e.g. if your heroku url is `my-echobot-app.herokuapp.com` you would use `http://my-echobot-app.herokuapp.com/listen` as the outgoing webhook url. Make sure you add `http` as well. __you must append /listen to the url in order for the app to hear the texts it is being sent__

![alt text][domains]

6) That's it, you're done! Send your newly configured Burner number a text and it should reply back. The first time you send a message it might take a few seconds to reply, so if it doesn't reply immediately be patient.

![alt text][screenshot]

[logo]: https://static.burnerapp.com/eb_wide.png "Echobot Logo"
[incoming]: https://static.burnerapp.com/echo_incoming_config.png "Incoming Webhook"
[manage]: https://static.burnerapp.com/echo_manage_heroku.png "Manage Heroku"
[domains]: https://static.burnerapp.com/echo_manage_domains.png "Find URL"
[screenshot]: https://static.burnerapp.com/echo_example.png "Echobot Example"
