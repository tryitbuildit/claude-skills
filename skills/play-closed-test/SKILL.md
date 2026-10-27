---
name: play-closed-test
description: Gets a new Android app through Google Play's closed test (12 testers opted in for 14 days) and ready to apply for production. Use when the user is publishing an app on a personal Google Play developer account, setting up closed testing, recruiting testers, tracking the 14-day counter, or preparing the production access application.
---

# Play Closed Test

Take an Android app from "uploaded" to "ready to apply for production" on a personal Google Play developer account, without restarting the 14-day clock.

## 1. Confirm the rule applies

Personal developer accounts created after November 13, 2023 must run a **closed test with at least 12 testers who stay opted in for at least 14 days in a row** before they can apply for production access. Ask the user which kind of account they have and when it was created. If the rule doesn't apply, say so and stop.

## 2. Set up the closed testing track

1. In Play Console: Test and release, Testing, Closed testing. Create or open the track, add the countries, and upload the release (an Android App Bundle).
2. For the tester list, recommend **one Google Group that anyone can join** over typed email lists. A group grows on its own, and you never edit the list again.
3. Warn the user:
   - A track uses email lists **or** Google Groups, not a mix.
   - Changing the tester list is a change Google has to review before it goes live.
   - Testers need a Google account; work or school addresses that aren't Google accounts are rejected.

## 3. Make one tester link

Build a single page (or message) with three numbered steps:

1. Join the Google Group.
2. Opt in at `https://play.google.com/apps/testing/<package.name>`.
3. Install the app from the Play Store link on the opt-in page.

Joining the group does **not** count. Only testers who tap opt in count toward the 12. Add a QR code for people reading on a computer.

## 4. Recruit with a buffer

- Aim for 15 to 20 opted-in testers, not 12. If anyone leaves while you sit at exactly 12, other developers report that the count starts over.
- Good free sources: friends and family with Android phones, tester-swap communities where developers test each other's apps, and a short post on LinkedIn or Reddit following each community's rules.
- Ask testers to open the app a few times during the 14 days and send one piece of feedback.

## 5. Track the counter

The Play Console dashboard shows how many testers are opted in and for how many days in a row. Check it every couple of days and write the numbers down. If the opted-in count drops toward 12, recruit more straight away.

## 6. Ship an update during the test

Release at least one update based on tester feedback while the test is running. The production application asks what you learned and what you changed, and a real update is the best answer.

## 7. Apply for production

When the dashboard shows 12 or more testers opted in for 14 days, apply for production access from the dashboard. Draft the answers with the user, honestly and specifically:

- How testers were recruited and how many took part.
- How they used the app and what feedback came in.
- What was changed because of that feedback.
- Why the app is ready for everyone.

## Gotchas

- In the store listing, words like "free" in the short description can be flagged as a price or promotion claim.
- In-app review prompts must not ask for 5 stars or offer rewards, and shouldn't be triggered from a button.
- A tester who installed a sideloaded build of the same app may see "Can't install" from Play, because Play builds are signed with a different key. Uninstall the sideloaded build first.

---

Want every form, message and fix ready to fill in? The full [App Launch Kit](https://tryitbuildit.com/launch-kit) adds every Play Console App content answer, tester posts and a 14-day tracker, production access drafts, rejection fixes and three checking tools.

Made by [Try It, Build It](https://tryitbuildit.com). More tested Claude skills: https://tryitbuildit.com/skills. Step-by-step app guide: https://tryitbuildit.com/guides/build-an-app-with-claude-code
