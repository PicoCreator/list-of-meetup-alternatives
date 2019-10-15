# list-of-meetup-alternatives
Compiling a list of meetup alternatives, and possible replacement technologies. PR is welcomed.

---

## Backstory

So meetup.com maybe planning to [charge a $2 per RSVP](https://meetup.com/lp/paymentchanges) - this will effectively kill any "free meetup". So as a meetup co-organizer myself, this is me researching for a plan to mitigate this!

---

## Open Source Solutions (with demo)

> The following are either outright meetup clones, or are "close enough" drop in replacement.

### Gettogether
[GIT](https://github.com/GetTogetherComm/GetTogether) - [DEMO](https://gettogether.community/teams/all/)

- **groups:** yes, with search (its a meetup clone)
- **event search:** yes, with locations, and more (its a meetup clone)
- **federation:** basic import from live sites, using a CLI command (on a cron schedule?)

Most feature complete, one-to-one with meetup.com, as it was part of its original design goals.

More importantly its the only project to recognize the need for federation of events.

### Agorakit
[GIT](https://github.com/philippejadin/agorakit) - [DEMO](https://app.agorakit.org/groups)

- **groups:** yes, with basic tag search
- **event search:** no (it does have calendars)

While the groups and event search is rather limited. Several additional functionalities are built in, rss, ical, and file management.

---

## "Incomplete" Open Source Solutions (with demo)

> The following tends to focus on either other challenges, or a narrow subsection of meetup feature set. This may on one hand make it an "incomplete" solution, but on the other hand for certain use caes, be much better suited.

### Gospeak

[GIT](https://github.com/loicknuchel/gospeak) - [DEMO](https://dev-gospeak.herokuapp.com/groups)

- **groups:** yes, with basic listing and search
- **event search:** no

This focuses more on the management of CFP's (Call for proposal), and have extreamly limited functionality around event lookup / rsvp

### Attendize
[GIT](https://github.com/Attendize/Attendize) - [DEMO](http://attendize.website/e/799/attendize-test-event-w-special-guest-attendize) - Attribution Assurance License

- **groups:** no
- **event search:** no

This is narrowly focused on managing the booking / ticket sales of an event page. So its not really a replacement.

## Open Source Solutions (upcoming / lacking info)

### eventoL
[GIT](https://github.com/EventoL/EventoL)

Very limited information in english, and without a live demo, may need help evaluating and filling in its features.

---

## Competitors

## Duck Taping / Ideas
