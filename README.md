# Fare-Bid Ride Bot

A concept for a Telegram ride bot where passengers name their price and drivers bid. The bot returns only what a passenger needs to choose: username, ride type, vehicle color and plate, fare, trip count and account age.

There are no human moderators. Trust comes from automatic rules:

- Drivers register with their permanent Telegram user ID and a photo of the car with the plate visible
- The bot sends the passenger that photo when a match is made, and holds the match until the driver shares live location
- Reminders go out at key moments (no prepayment, check the plate, screenshot the live location)
- After each trip, both sides rate each other; trip count and rating feed every future bid line
- A rule-based cooldown hides accounts that collect too many reports

## Workflow map

`index.html` is a self-contained, interactive swimlane map of the flow (Passenger / Bot / Driver, 10 steps). Open it in a browser or embed it:

```html
<iframe src="index.html"
        style="width:100%;height:1150px;border:0;border-radius:12px"
        title="Fare-Bid Ride Bot workflow" loading="lazy"></iframe>
```

Sample data on the page is made up.
