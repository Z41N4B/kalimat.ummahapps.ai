# Kalimat كَلِمَات

A free Arabic vocabulary trainer for beginners. Live at https://kalimat.ummahapps.ai/

**Words:** over 400 everyday words with full harakat, in 16 groups (basics, people, places, home and school, food, nature and animals, body, colours, describing, actions, numbers, time, greetings, clothes, toys, feelings).

## Features
- Tap any word to hear it, at normal or slow speed (uses the device's Arabic text-to-speech voice)
- Sound and broken plurals for most nouns and describing words
- Words sorted from Beginner to Advanced, with a level filter
- Qur'an words list (from "80% of Qur'anic Words"), with both meanings on shared words
- Verb forms: past, present, command, doer and action noun
- Stories: 15 short, fully vowelled stories made mostly from words in Kalimat, including 5 funny versions that repeat the words of the story before them. Listen first with pictures, read along and tap any word for its meaning, answer questions in Arabic, then tell the story yourself. Each story shows how many of its words you already know, suggests a good next story and offers to add its new words to Learning.
- Games: pick the picture, build the word (tap its letters in order, with أحسنت and stars for each word), pick the plural, pick the form, say it from memory, say the plural from memory, revise known words, with an optional 10 or 20 second timer
- A button that jumps to the bottom of the long pages and back to the top
- A progress card on every tab: words known well out of the total, the percentage, the next goal, and more detail for each word list and the stories
- Mark the words you are learning, then mark them as known well (or get a word right first time 5 times in a row, in the games or story questions, and it moves there by itself)
- Spaced checks on Known well words: after 3 days, 1 week, 2 weeks, 1 month and 2 months
- Add your own words
- Up to 3 learners on one device, each with their own progress, shared with Takallum Kids, Kalimat Plus and Takallum
- Words known from the other apps: a note on the Words tab offers to add them to Learning
- A short note on sound and broken plurals, on the Words tab and in the two plural games

## Shared with the other apps
Takallum Kids, Kalimat, Kalimat Plus and Takallum share three things on the same device through `ummah.js`, which is copied into each app's folder (keep the four copies identical):
- **Learners:** name, boy or girl (man or woman), and animal, in the `ua_l` cookie on `.ummahapps.ai`. A learner added in one app appears in the others; a learner still called "Learner 1" stays in its own app until renamed.
- **Known words:** words learned in Takallum Kids and Known well words in Kalimat and Kalimat Plus go into a per-learner `ua_w_<id>` cookie as short hashes of the bare Arabic. Kalimat and Kalimat Plus offer to add words known from the other apps.
- **Settings:** voice speed (slow, normal, natural), playing the Arabic straight away and vowel marks go with each learner in a `ua_s_<id>` cookie (`ua_s_d` for a learner with no name yet), and the voice help goes with the device in `ua_d`. The Settings panel that changes them is drawn by `ummah.js`, so it is the same in all four apps; each app opens it from its learner row or settings sheet and turns the speed into its own voice rate. The first time an app loads the shared settings, what was set in that app before fills in for the learners already on the device; new learners start from the defaults.

Each page also ends with the same four-app family strip. On localhost, `ummah.js` points the strip's links at the local servers (Kids 8771, Kalimat 8766, Kalimat Plus 8772, Takallum 8770).

## SEO and GEO
`index.html` has meta tags, Open Graph and JSON-LD (WebApplication + FAQPage). `robots.txt`, `sitemap.xml` and `llms.txt` sit at the root.

## Running locally
```
node serve.js
```
Then open http://localhost:8765
