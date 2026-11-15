# Mars Outpost

**NASA Space Apps Challenge 2026 | Challenge: Space Mission Design Game | Team: System-Error 404**

Astronauts crash-land on Mars. Their ship is wrecked, and the only way home is to rebuild it. Mars Outpost is a pixel-art survival game that teaches how a real Mars mission works: managing scarce resources, living with space weather, defending a base, and collecting the parts to launch home.

- **Play the game:** https://skyfiredragon22.github.io/NASA-Space-Apps-Game-Idea-SYS-Error-404/
- **Watch the 30-second trailer:** [mars-outpost-trailer.mp4](mars-outpost-trailer.mp4)
- **Source code:** https://github.com/SkyfireDragon22/NASA-Space-Apps-Game-Idea-SYS-Error-404

## The challenge

Design a game that lets players plan and run a space mission. We chose the hardest part of any Mars mission: staying alive long enough to get home.

## Our solution

You command a stranded outpost. You start with three days of supplies. To get home, you have to find, earn and build five rocket parts. Along the way, the game teaches real space science.

- **Survive:** Keep air, water, food and power up. Run out of any of them and the crew is in trouble.
- **Face real space weather:** Solar flares, coronal mass ejections (CMEs) and Mars dust storms hit the outpost, draining power and shields. The events are modelled on real NASA space-weather data from the DONKI database (Space Weather Database Of Notifications, Knowledge, Information).
- **Defend the base:** A radar warns of incoming creatures. Build tower-mounted weapons, shields and upgrades, and fight several enemy types, each with its own attacks and drops.
- **Learn to earn:** Quizzes and Captain Nova's daily fun facts teach real NASA science. Correct answers earn the supplies you need to rebuild.
- **Grow the base:** Mines, drills, life support, a power generator and an inventory open up gradually, a few mechanics at a time, so new players are never overwhelmed.
- **Rebuild the ship:** Collect five rocket parts, then launch for home.

## How to play

1. Open the game link above. Any modern browser works, on a computer or a tablet.
2. Turn the sound on for the narrator.
3. Follow the short tutorial on day 1. Your first goal is to get through the first three days.
4. Use the buttons at the edge of the screen for the inventory, quests, mines, upgrades and defense.
5. Answer quizzes, finish quests, build the ship parts and fly home.

To play offline, download this folder and open `index.html`. Keep the `audio` folder beside it so the narrator works.

## What players learn

- Why astronauts need a steady supply of air, water, food and power
- How solar flares and coronal mass ejections affect missions
- What dust storms do to solar power on Mars
- Why a mission needs planning, trade-offs and backup plans
- Fun facts about NASA spacecraft, rovers and the Sun

## Built with

- HTML, CSS and JavaScript in a single page, with no installs and no server needed
- Canvas pixel-art graphics
- Narration recorded with ElevenLabs text-to-speech
- Original sound design and music, synthesized in Python
- GitHub Pages for hosting
- AI-assisted development using Claude

## Data and credits

- NASA DONKI space-weather database (solar flares, CMEs and geomagnetic storms), as inspiration for the in-game events
- NASA Mars mission science facts used in the quizzes and tips
- Narrator voice: ElevenLabs

## Files

| File or folder | What it is |
| --- | --- |
| `index.html` | The game |
| `audio/` | Narrator voice recordings (149 files) |
| `mars-outpost-trailer.mp4` | The 30-second trailer |
| `trailer-script.txt` | The trailer narration |

## Team

**System-Error 404:** _add team member names here_


## Courtesy of Claude: Prompts


 **Mars Outpost Game Prompts**
The prompts used to build the Mars Outpost game, in order.

  **1. Create the game**
Attached design files: Mars Outpost Game UI Final.pdf and Mars Outpost Game UI Final.html

create an educational game for young children. The design is linked, one as a pdf, one as an html. The game info is here:

  Story Line: On Mars, a group of explorers/settlers try to defend the outpost from aliens while managing resources, upgrades, and technology to survive. Aliens also get more advanced tech. Aliens come in waves; no aliens for the first 5 days. They attack randomly. Use the downtime to prepare; natural disasters can also occur, though less likely/frequent. Like dust storms, fires, marsquakes, and meteor strikes.

  Create an outpost on Mars; don't know the strength of aliens yet, thought that we would be able to overcome them. For the first 5 days, aliens don't know we are invading, but they send a small group of weaker ones as scouts because they sense an anomaly on the planet. We are scouts too for further invasions. No access to Earth resources for the time being, want to return to Earth but spaceship broke down.

  Aliens drop resources; low-level ones drop food, water, contained air; medium ones drop power cells, metals; bosses drop uranium and life support

We start with 1 life support, 3 days of basic life needs and electricity, and basic defenses.

  Life support: increase power, food, water, and air by a tiny bit and has a refresh time of 3 days

10 min irl = 1 day simulation 5 min day, 5 min night

Quests to understand more about terrain and aliens which helps increase defense level by a bit

Pixel art

Pixel Game

Mines - building to put drills in (basically afk mining) gets us minerals that we need

Levels:

Electricity Levels:

Wood
Coal/gas
Biofuel(so not just any organic material, alien biofuel from ships)
Solar panels
Nuclear power plant
Defense Levels:

Offensive
Guns
Weapons(in general)
People
Robots
Lasers
Plasma
Emp
Gravitational control
Defensive(shields) - level up to be able to take more damage
Wall (physical dome)
Electromagnetic shield
Fungal shield(fungi absorb radiation)
Gravitational shield
Plasma shield
Basic life needs:

Water
Charcoal
Rocks
Reverse osmosis
Biological neutralization? Bacteria eat germs and organic stuff
Food
Basic plants - veggies
Add kitchen here
Spirulina - more nutritious
Cloned + genetically modified animals
Air
Plants
Electrolysis
MOXIE - turns CO2 into oxygen
Life support: the more we have the more efficient and faster it is

Resources:

Defenses, to aliens AND radiation(defense does both at the same time) made of steel, tech
Basic life needs - food, water, air
Power - electricity
Life support (Sustain Life)
End: gain enough resources to build a rocket and then leave Mars and return to Earth, which makes it the end

**2. Hard choices, constant power drain, solar flares, faster speeds**
add parts where each choice has to make players consider the sacrifice of doing it or not, power must decrease all the time, we choose when to generate more food or water or air or replenish defence and it costs us power, have no safe choices, also make the time be able to speed up faster. every single choice we make deplets another resource, add solar flares(don't need a design) that makes our power and defense go down

**3. Punishments for empty resources**
ok we need a punishment if we run out of any of these...

**4. Slow down during danger**
also can you make the game slow down to x1 speed when fire, meteor(natural disaster) or alien attacks come then return to the old speed when it's over?

**5. Allow speeding up again during danger**
ok so make it so that we can make the speed increase after putting it at x1(so like if its a dust storm, reset it to x1, then we can click on the speed to increase if we want)

**6. Real NASA solar flare and interplanetary shock data**
add this data for solar flare: curl --request GET --url 'https://ccmc.gsfc.nasa.gov/DONKI-API/get/FLR?startDate=2016-01-01&endDate=2016-01-30'
also add ips(interplanetary shocks) into it(decrease power and defense by A LOT) but have them really unfrequent(data is here, use it): curl --request GET --url 'https://ccmc.gsfc.nasa.gov/DONKI-API/get/IPS?startDate=2016-01-01&endDate=2016-01-30'

**7. Keep the real day-1 flare**
Keep it on day 1

**8. Kid-friendly wording**
make the information less techy so that kids can actually understand it

**9. Shorter days**
change length of 1 day to 2min, keep proportions(1min day, 1 min night)

**10. Optional tutorial, fewer pop-ups, explain MOXIE**
can we make captain nova's information not pop up so often? so like at the beginning of the game as a tutorial(let players choose if they want a tutorial) and after that don't have it pop up every time we get materials from the mine, etc. also explain what moxie is.

**11. Save the prompts**
can you save the prompts here to a new file called "mars Outpost Game Prompts"

**12. Restart button, save codes, clearer tutorial, text to speech**
make a restart game button, also, for each new game, create a code that u can enter at the home screen to be able to continue an old game. also, make a clearer tutorial and game purpose, add text to speech to it

**13. Save codes on any device**
Yes, any device

**14. Tutorial detail, pop quizzes, more metal**
really make each function clear in tutorials
pop up random questions occansionally that give u more energy, food, water, or air
let us get a lot more metal
from drills

**15. Daily biofuel from waste**
generate biofuel(like from waste) every day(like 2 biofuel a day)

**16. Intro video, music, hands-on tutorial**
add a like intro video that shows us the whole premise of the game and what happens before. add cool background music. so kind of like champion's island google doodle style? clearly show how to make some resources. in the tutorial make people click on buttons(like u have to click into upgrades and buy biofuel, etc)

**17. Ending cutscene**
add cutscene at the end too


