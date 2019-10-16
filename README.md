# list-of-meetup-alternatives
Compiling a list of meetup alternatives, and possible replacement technologies. PR is welcomed.

---

## Context

So meetup.com maybe planning to [charge a $2 per RSVP](https://web.archive.org/web/20191014205500/https://www.meetup.com/lp/paymentchanges) - this will effectively kill any "free meetup". So as a meetup co-organizer myself, this is me researching for a plan to mitigate this!

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

### open-event
[GIT frontend](https://github.com/fossasia/open-event-frontend) - [GIT backend](https://github.com/fossasia/open-event-server) - [LIVE](https://eventyay.com/)

- **groups:** no
- **event search:** yes

FossAsia (great folks) very own event organization platform, while it lack "groups" and subscription to groups. From an event organizer perspective it is full of additional features, including but not limited to, ticket billing, call for speakers handling.

### Agorakit
[GIT](https://github.com/philippejadin/agorakit) - [DEMO](https://app.agorakit.org/groups)

- **groups:** yes, with basic tag search
- **event search:** no (it does have calendars)

While the groups and event search is rather limited. Several additional functionalities are built in, rss, ical, and file management.

### Mobilizon 
[GIT](https://framagit.org/framasoft/mobilizon/) - [DEMO](https://test.mobilizon.org/events/f2fd4a0c-64c2-46a4-bc47-b61c087234de)

- **groups:** yes, with basic tag search
- **event search:** yes, with location, and keywords

Provides basic discoverability features, for related event. Currently in extremely early beta phase.

### on_ruby
[GIT](https://github.com/phoet/on_ruby) - [LIVE](https://www.onruby.eu/)

- **groups:** yes, no search
- **event search:** no

While this may seem feature "incomplete" it might be good enough, for a small group (<100) of strongly interelated communities. From then each group has full functionality, to organize events, and subscribe to news / etc.

### Swachalit
[GIT](https://github.com/null-open-security-community/swachalit) - [LIVE](https://null.co.in/)

Simliar to on_ruby, where it may work strongly for a small collection of groups. It has extensive feature within a group.

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

---

## Open Source Solutions (upcoming / lacking info)

> Either in early stages or lack a working english demo to do assessment - may need feedback from others

### eventoL
[GIT](https://github.com/EventoL/EventoL)

Very limited information in english, and without a live demo, may need help evaluating and filling in its features.

### Chapter
[GIT](https://github.com/freeCodeCamp/chapter)

Very initial stages, of freeCodeCamp attempt to build their own platform.

---

## Not Exactly Competitors

> Interesting alternatives that have been used to organize events. Without most of the features provided. But it works! In a hackerish sort of way.

### Facebook

This is already a common alternative for non-tech events. While it enjoys the benefit of sharability on the much larger social network.
The downside is that it limits searchability of event attendess. I need to know / be in the group, to manually check for events.

That being said - it is facebook, the largest platform there is. So pros, and cons.

### Github

While an un-orthodox alternative, this does tap on to a large existing developer focus community space.
With all the downsides as mentioned in facebook.

There have been good examples though, such as [kopi.js](https://github.com/KopiJS/kopi.js/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aclosed+)

---

## Competitors

> Out right, full commercial replacement / competitor. 

### Eventbrite

They focus on events first, with very limited search by tags. And no support for groups, meaning no subscription of groups.

Well established in the events and ticketing space

### kommunity.com

Seems like a meetup.com clone that is starting out

### [Meetabit](https://meetabit.com)

Aimed at technical meetups, and backed by some of their organizers. While it lack in-depth search and discoverability.
It includes additional features like: accept talk proposals and sponsorship offers, archive of talks and related materials and export data. And is taking an interesting alternative approach to the layout of information (aka not a clone).

### [opensports.net](https://opensports.net)

Sports focused alternative, with membership subscription optons (like gym?) - I do not know, might need more info.

### [emamo.com](https://emamo.com)

Looks pretty, and is focus more on a platform for large event / conference organizer, with established consumer. Rather then a platform for consumers.

---

## Competitors Launching Soon

> New, Shiny, unknowns. Have to wait and see.

- https://cete.io/
- https://eventy.io/

---

## Personal Notes

While the developer in me might want to jump to "lets open source" this.

It is important to recognise that the success of meetup.com, to an event organiser is that it is "a social network" focusing on well - meetups.

Its biggest strength was that attendees of any events, can randomly discover other related events by subscribing to an existing group, or by searching for it. 

There are several expensive event management system with superior features, but without the social network.

Having every organizer hosting their own "meetup server" is probably a worse case scenerio, as it effectively kills off the ability for small organisers (<10 attendees) from getting off the ground. 

Likewsie having all the tech organizer going over to 101 competitors, will impact us due to fragmentation of the community.

So in my oppinion having a feature complete meetup.com clone is not a solution.

- It has to be easy for **any** organiser to spin up (not a sysadmin).
- It has to have discoverability built in to other events, beyond the one being organized.
- It has to have a subscription feature for attendees of groups to keep track of upcoming events, they subscribed to. (Full raw list is too much)

A possible solution is to have multiple major hubs interconnected. With major organizer forming their own hub. Commonly refered to federation, however this requires a logistical work on hub administrator to interlink / etc.

Unfortunately, the laziest effective solution tends to work here. And this makes it heavily favour a commercial or community-sponsored owner, who will have the time and energy to focus on making sure it "just works"

And as an event organiser, there does not seem to be an alterantive now. While facebook is able to resolve the social network side of the equation, it is hardly a meetup search and management tool.
