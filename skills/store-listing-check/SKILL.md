---
name: store-listing-check
description: Reviews or writes a Chrome Web Store or Google Play listing to catch common rejection causes before you submit. Use when the user is preparing, reviewing or fixing a store listing, responding to a store rejection, writing permission justifications, or filling in a privacy or data safety form for a Chrome extension or Android app.
---

# Store Listing Check

Check a Chrome Web Store or Google Play listing against the mistakes that most often get new developers rejected, then rewrite what needs fixing.

## Inputs

Ask for (or read from the project): the store, the listing text (title, short and full description), the permissions or data the app uses, the privacy policy URL, and the screenshots. If the user only has an idea, write the listing from scratch using the same checks.

## Chrome Web Store checks

- **No lists of other brands, sites or products** in the description ("works on Site A, Site B, Site C..."). Lists like this are treated as keyword spam and can get an instant rejection. Describe what it does instead.
- **One clear purpose,** stated in the first sentence. Every feature should serve it.
- **Narrowest permissions.** Remove anything unused. Prefer optional or activeTab-style access over access to all sites. Write one plain-English justification per permission.
- **Privacy:** the data usage answers must match what the code actually does and what the privacy policy says. The privacy policy URL must be live.
- **No implied affiliation** with brands the extension works with. Add "not affiliated with ..." where it helps.
- **Screenshots:** use your own footage or properly licensed material with credit, not someone else's copyrighted video.

## Google Play checks

- **Title** within 30 characters, **short description** within 80. No promotional or price words such as "free", "best" or "#1" in the title or short description; they can be flagged.
- **No asking for ratings** with incentives, and no "give us 5 stars".
- **Data safety form** matches everything the app and its SDKs collect (ads, analytics, crash reporting, accounts).
- **Content rating** questionnaire answered honestly. Chat or user interaction features change the rating.
- **Graphics:** a 512x512 icon, a 1024x500 feature graphic and at least two phone screenshots.
- **Privacy policy** linked and live, and the account deletion link provided if the app has accounts.

## Output

Return three sections:

1. **Must fix:** anything likely to cause a rejection, quoting the exact line.
2. **Should fix:** things that weaken the listing (vague first sentence, missing benefit, weak screenshots).
3. **Ready to paste:** the corrected title, short description and full description, each within the store's character limits, plus permission justifications if needed.

Keep every claim true. Don't invent user counts, ratings or awards.

---

Want the full version? The [App Launch Kit](https://tryitbuildit.com/launch-kit) adds ready-to-fill Chrome and Play templates, every Chrome rejection code with its fix, real approved examples and three checking tools.

Made by [Try It, Build It](https://tryitbuildit.com). More tested Claude skills: https://tryitbuildit.com/skills
