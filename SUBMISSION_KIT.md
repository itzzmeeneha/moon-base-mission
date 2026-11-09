# Submission kit: Moon Base Mission

Fill in the parts in angle brackets. Check the official submission form for the exact fields and limits, because they can change.

## 1. Title and one-line summary

**Title:** Moon Base Mission

**One line:** A browser game where kids aged 7 to 12 run a Moon base for twelve days, sharing limited power between air, a radiation shield and science, while solar storms based on real NASA flares test their choices.

## 2. Short description (about 120 words)

Moon Base Mission teaches the real trade-offs of surviving on the Moon. Players get a few units of power each day and must split them between life support, a radiation shield and science. Nothing is free: science earns points but leaves less for safety, and saving power for the long lunar night means giving up points today. Three solar storms hit during the 12-day mission, and each one is based on a real flare from NASA's DONKI space weather database, shown with its real class and date. A stronger shield means less harm to the crew. Every game is different, and a mission report at the end shows what happened. It runs in any browser with no download or account.

## 3. Long description

**The problem.** Space education for kids is often either posters full of facts or simulations built for engineers. Few tools let a young player feel why astronauts have to make hard choices with limited power.

**Our solution.** A simple turn-based game with only three systems, so a 7-year-old can understand it. Each day the player places power cells on life support, the radiation shield or the science lab. Before they commit, each row shows what tonight's result will be, so the cost of every choice is visible.

**The trade-offs it teaches.**
- Power is shared. More science means less safety.
- The Moon's night lasts about 14 Earth days, so solar panels stop working. Players must save power in a battery during sunny days.
- The crew uses air every day and the shield wears down, so standing still means falling behind.
- Radiation from the Sun varies. A stronger shield means less damage from a storm.

**How we use NASA data.** When the game loads, it asks NASA's DONKI solar flare API for flares from the last 30 days. Each storm in the game is one of those real flares, and the flare's class (C, M or X) sets the storm's strength. The alert shows the flare's class and date so players can see it is real. If live data cannot be reached, or the Sun has been quiet, the game uses a saved list of real flares from 2024 and labels them as archived.

**What is simplified.** The air, shield and damage numbers are game balance, not engineering values. In the game every storm hits at the end of a day, while in reality flare radiation can arrive within minutes to hours.

**Replayability.** The storm days, the real flares chosen, the length of the sunny period, moon dust and air leaks are all randomised each game. Losing shows a gentle message about what to try next.

**What's next.** A Mars mode with a communication delay, more NASA data such as astronaut health findings from OSDR, and difficulty levels.

## 4. Demo video script (about 3 minutes)

Record your screen with a voiceover. Keep it calm and clear.

| Time | Show | Say |
|---|---|---|
| 0:00 to 0:20 | Title screen | "This is Moon Base Mission, a game that teaches kids how astronauts share limited power to stay alive on the Moon. I'm `<your name>` from team `<team name>`." |
| 0:20 to 0:50 | Game screen, point at the three rows | "Every day you get a few power cells. Life support keeps the air up, the shield protects the crew from radiation, and science earns points. There is never enough for everything." |
| 0:50 to 1:20 | Place cells, point at the "tonight" text | "Before you commit, each row shows what tonight's result will be, so the cost of every choice is clear." |
| 1:20 to 1:50 | Timeline strip and battery | "The Moon has a long night when the solar panels stop working. You need to save power in the battery during sunny days." |
| 1:50 to 2:25 | A storm alert, then end the day | "This alert is based on a real solar flare from NASA. It shows the real class and date. A stronger shield means less harm to the crew." |
| 2:25 to 2:45 | Mission report screen | "At the end, a mission report shows what happened, including the real flares the crew faced. Players can save it as an image." |
| 2:45 to 3:00 | Footer credit | "The data comes from NASA's DONKI space weather database. The game runs in any browser with no download. Thank you." |

Tips: play one practice game first so you know what will happen. Use headphones off the mic to avoid game sound in the recording, or turn sound off with the button at the bottom right.

## 5. Checklist before you submit

- [ ] Game is online (GitHub Pages link opens and works in a fresh browser tab)
- [ ] README has the live link and your AI-use note filled in
- [ ] Video is uploaded and its link opens without signing in
- [ ] Project page lists the NASA data used: DONKI solar flares
- [ ] The data status line shows green "Live data" when you test with your own API key
- [ ] You tried it on a phone
- [ ] Team members are added on the Space Apps site

## 6. AI-use note (be honest and specific)

Space Apps asks teams to disclose AI tools. Write what is true for you. A draft you can edit:

> We used Claude (Anthropic) to help plan the game, write the code, and design the interface. We tested the game ourselves and chose the final design and rules. NASA's DONKI data and the facts in the game were checked against public sources.

Only keep the last sentence if you really did check them. You should be able to explain how your game works, so read through `index.html` and ask for explanations of any part you don't understand before judging.

## 7. Questions judges may ask

- **Which NASA data did you use and why?** DONKI solar flare data, because radiation from the Sun is a real danger on the Moon and it lets the game reflect real space weather.
- **Is the data live?** Yes when the NASA API can be reached. If not, the game uses archived real flares and labels them as archived.
- **What does a young player learn?** That power is limited, that the lunar night needs planning, and that shielding is a real trade-off.
- **What is simplified?** The numbers are game balance, and storms hit at the end of each day.
- **What would you add next?** A Mars mode with communication delay and more NASA datasets.
