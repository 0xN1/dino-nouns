# dino-nouns

![Image](https://cdn.discordapp.com/attachments/1014135287087108196/1026983796152746004/unknown.png)

DinoNouns(working title). An interactive NFT project by Nero One based off [nouns](https://nouns.wtf) dino head

# Ideas
I've worked on several Interactive NFT project and most of it was off-chain, [COMLINK+](https://opensea.io/assets/ethereum/0x1b7e73c6d30dd5dd811cbd26d9bf36e34882fd39/3)(pointed to a website), [tulsv1](https://exchange.art/editions/HkMrXQ7NRZy7UuSvLSpW8Vhut7ZnPn9phRYKerCZ8uba)(uploaded to IPFS).

However this time I wanted to put the whole HTML on-chain + interactive.

The only off-chain solution would be the CloudNouns API for SVG generation.

So to achieve this, all asset need to be encoded in base64, including all the fonts. The HTML will be using vanilla HTML to make it simple as possible without any other dependencies.

## Features
- Text-based command interaction
- Uses [CloudNouns](https://cloudnouns.com) API to generate new Dino nouns
- Dino stats
- Basic Gamification
- Uses local storage for data
- Dynamic favicon and title
- Utility commands like `/help`, `/reset`
- more..

## Progress
- Basic command setup
- Call CloudNouns API to get SVG
- Simple UI
- STR and AGI stats
- `/jump` & `/run` command
- Age stat changes over time
- New design mockup
- Code refactor
- Commands now has random rate to fail

# Demo
[DinoNouns](https://recondite-flame.surge.sh)

# Installation

Clone repo

`git clone https://github.com/0xN1/dino-nouns.git`

Install packages

`npm install` / `yarn install`

Run the webserver

`npm run start` / `yarn start`

---
## TODO
- randomisation for command usage [x]
- lowercase every command [x]
- add icons for the stats, preferably 1-bit
- use latest design mockup
- dino reaction text
- WIP


## FUTURE
- utils cmd for nounish stuff
- cmd to map button
- use keyboard
- use gamepad api 
- chrome extension?
