# Submission kit: Moon Base Mission

Fill in the parts in angle brackets. Check the official submission form for the exact fields and limits, because they can change.

## 1. Title and one-line summary

**Title:** Moon Base Mission

**One line:** A browser game where young astronauts-in-training run a Moon base for twelve days, sharing limited power between air, a radiation shield and science while solar storms built from real NASA flare data test their choices, then test their strategies like scientists in the Mission Lab.

## 2. Short description (about 120 words)

Moon Base Mission teaches the real trade-offs of surviving on the Moon. A friendly guide, Pip, trains players with a short briefing and then gives advice every day. Players split a few power cells between life support, a radiation shield and science. Three solar storms hit during the mission, each based on a real flare from NASA's DONKI space weather database, shown on a live chart with its class, date and a link to the NASA record. An international crew writes a log that turns every choice into a story. In the Mission Lab, players make a hypothesis, run a fair test of 2,000 simulated missions and draw a conclusion. The game ends by connecting the lessons back to life on Earth. It runs in any browser, with no download or account.

## 3. Long description

**The problem.** Space education for kids is often either posters full of facts or simulations built for engineers. Few tools let a young player *feel* why astronauts make hard choices, or show that real NASA data is something they can explore themselves.

**Our solution.** A turn-based game with only three systems, so a 7-year-old can understand it, plus a guide character who never leaves the player alone.

- **Training first.** A 7-step briefing (with a practice row) explains everything before the mission. On the first mission, Pip highlights each part of the screen.
- **Advice that reacts to the player's plan.** Before the player ends the day, Pip warns them if the air will run out, how much harm tonight's storm will do at the current shield level, or when the lunar night is close.
- **Real data, made visible.** Live solar flares from NASA DONKI drive the storms and are plotted on a chart of flare strength. Each storm links to its NASA record.
- **The scientific method.** The Mission Lab walks through question, hypothesis, experiment and conclusion. The experiment is a fair test: every plan faces the same 500 missions.
- **Story and connection.** A crew from India, Canada, Japan and Brazil writes a daily log that reacts to what happened.
- **Back on Earth.** The debrief connects the lessons to solar power and batteries in remote communities, space weather's effect on satellites, GPS and power grids, and sharing limited resources.

**What is simplified.** The air, shield and damage numbers are game balance, not engineering values. Storms hit at the end of a day, while in reality flare radiation can arrive within minutes to hours. The crew names are fictional.

## 4. Which awards this project fits, and why

Use these points in your project description and in the video. Only claim what you can show.

| Award | What to point judges to |
|---|---|
| **Best Use of Science** | The Mission Lab follows the scientific method step by step: question, hypothesis, a controlled experiment (same 500 missions for every plan, only the plan changes), results chart, and a conclusion that says honestly whether the hypothesis was supported. The surprising result (the "obvious safe" Steady plan survives only about 10% of the time) teaches why testing beats guessing. |
| **Best Use of Data** | Live NASA DONKI flare data drives the game, is plotted on a flare-strength chart with C/M/X bands, and links to each flare's NASA record. Archived data is always clearly labelled as archived, never passed off as live. |
| **Best Use of Storytelling** | Pip's briefing and advice, the crew log reacting to each event, and the debrief turn data into a story: a real X-class flare becomes "That storm hurt us badly". |
| **Art & Technology** | Every visual is hand-built SVG (Pip, the crew, the Moon scene, the charts) and every sound is generated live in the browser, all in a single HTML file with no images, sound files or libraries. |
| **Global Connection** | An international crew, real global space-weather data, and a game that works on any browser in the world with no install or account. |
| **Local Impact** | One small file that works offline (with archived NASA data) on low-cost phones and school computers, so schools with weak internet can still use it. `<Add your local plan here, for example: tested with students at a Chennai school or club, and what they said.>` |
| **Galactic Impact** | The "Back on Earth" section links the game to solar power for off-grid communities and to protecting satellites, GPS and power grids from space weather. |
| **Most Inspirational** | Pip makes a first-time player feel capable: nobody is thrown in without help, and losing ends with an encouraging tip, not a failure screen. |

Pick **two or three** of these to lead with, rather than claiming all of them. The strongest fits are probably **Best Use of Science**, **Best Use of Data** and **Best Use of Storytelling**.

## 5. Demo (the form allows ONLY a 30-second video OR up to 7 slides)

To be eligible for a Global Award, the demo must be **no more than 7 slides** or **no longer than 30 seconds**, at a public link that needs no sign-in.

**Option A (ready to use):** the 7-slide PDF in `demo/Moon-Base-Mission-demo.pdf`. Link it from GitHub.

**Option B: 30-second video script** (screen recording with voiceover):

| Time | Show | Say |
|---|---|---|
| 0 to 5 s | Title screen with Pip | "Moon Base Mission: a trainer for young astronauts." |
| 5 to 12 s | Place cells, Pip's warning changes | "Share limited power between air, a radiation shield and science. Pip, your guide, warns you before things go wrong." |
| 12 to 20 s | Storm alert, then the flare chart | "Solar storms come from real NASA DONKI flare data." |
| 20 to 27 s | Mission Lab results | "In the Mission Lab, you test strategies like a scientist, with a fair test of 2,000 missions." |
| 27 to 30 s | Game link on screen | "Free, in any browser. Play it now." |

If you make a video with any AI tool, the rules require a visible watermark saying it is AI-generated.

## 6. Checklist before you submit

- [ ] Game is online (GitHub Pages link opens and works in a fresh browser tab)
- [ ] README has the live link and your AI-use note filled in
- [ ] Demo (7 slides or 30-second video) link opens without signing in
- [ ] Project page lists the NASA data used: DONKI solar flares (plus OSDR, RadLab and CSA as background for facts)
- [ ] The data chip shows "Live data" when you test with your own API key from api.nasa.gov
- [ ] You tried it on a phone
- [ ] You ran the Mission Lab once and can explain why the results came out that way
- [ ] Team members are added on the Space Apps site

## 7. AI-use note (be honest and specific)

Space Apps asks teams to disclose AI tools. Write what is true for you. Here's a draft you can edit:

> We used Claude (Anthropic) to help plan the game, write the code, and design the interface, including the guide character and the Mission Lab. We tested the game ourselves and chose the final design and rules. NASA's DONKI data and the facts in the game were checked against public sources.

Only keep the last sentence if you really did check them. You should be able to explain how your game works, so read through `index.html` and ask for explanations of any part you don't understand before judging.

## 8. Questions judges may ask

- **Which NASA data did you use and why?** DONKI solar flare data, because radiation from the Sun is a real danger on the Moon. It drives the storms, and players can see it on a chart and open the NASA records.
- **Is the data live?** Yes, when the NASA API can be reached. If it can't, the game uses archived real flares from 2024 and labels them as archived.
- **How is the Mission Lab a fair test?** Each of the 500 missions uses a fixed random seed, so every plan faces exactly the same storms, days and events. Only the plan changes.
- **What does a young player learn?** That power is limited, that the lunar night needs planning, that shielding is a trade-off, and how to test an idea with an experiment.
- **What is simplified?** The numbers are game balance, storms hit at the end of each day, and the crew is fictional.
- **What would you add next?** A Tamil and Hindi version for local schools, a Mars mode with a communication delay, and astronaut health data from OSDR.
