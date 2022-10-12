# dino-nouns

A ⌐◨-◨ work in progress

![Image](https://cdn.discordapp.com/attachments/1014135287087108196/1028545362522292244/unknown.png)

DinoNouns. An onchain, dynamic and interactive NFT project by Nero One based off [nouns](https://nouns.wtf) dino head

# Ideas
I've worked on several Interactive NFT projects and most of it was off-chain, [COMLINK+](https://opensea.io/assets/ethereum/0x1b7e73c6d30dd5dd811cbd26d9bf36e34882fd39/3)(pointed to a hosted site), [tulsv1](https://exchange.art/editions/HkMrXQ7NRZy7UuSvLSpW8Vhut7ZnPn9phRYKerCZ8uba)(uploaded to IPFS).

However this time I wanted to put the whole HTML on-chain + interactive.

So to achieve this, all asset need to be encoded in base64. I'm using vanilla HTML, CSS and JS to make it simple as possible without any other dependencies.

I'm currently using NounsDescriptor contract to generate onchain SVG for DinoNouns. 

Dino name is stored onchain and to change, you're required to interact with the DinoNouns contract. Changing name will reroll the Dino.

## Features
- Text-based command interaction
- Uses NounsDescriptor contract to generate new Dino nouns
- Dynamic onchain name
- CSS Animation
- Basic Gamification
- Dynamic favicon and title
- Utility commands like `/help`, `/reset`, `/map`
- Commands have `30%` chance to fail
- Teach your dino words!
- more..

---

## Commands

List of commands

| Command | Desc | Usage | eg|
|-|-|-|-|
|/dino|create your dino|/dino [name]|/dino abu|
|[any]|dino will say it back|[any]|hi|
|/run|make dino run|/run|/run|
|/jump|make dino jump|/jump|/jump|
|/clear|clear logs|/clear|/clear|
|/reset|reset to default dino|/reset|/reset|
|/map|map command to button|/map [btn][command]|/map a run|
| ~~/dl ~~| ~~download your dino SVG file ~~| ~~/dl ~~| ~~/dl ~~|
| /teach| teach your dino words!|/teach [word] [reply]| /teach yo whatsupp!|

## Demo
[DinoNouns](https://recondite-flame.surge.sh)


## Installation
Clone repo

`git clone https://github.com/0xN1/dino-nouns.git`

Install packages

`npm install` / `yarn install`

Run the dev server

`npm run start` / `yarn start`

Build for production. File will be created in `dist`

`npm run build` / `yarn build`

---

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
- randomisation for command usage
- lowercase every command 
- use latest design mockup
- dino reaction text
- cmd to map button `/map`
- keyboard shortcut, A,B,X,Y button mapped to responding keys
- optimize HTML and deploy renderer contract in Solidity
- dino name on-chain. change name need to interact on-chain
- use onchain svg from nouns contract

## TODO
- add icons for the stats, preferably 1-bit
- stats creation and manipulation
- add solidity contracts
- instructions to fork

## FUTURE
- utils cmd for nounish stuff
- use gamepad api 
- chrome extension?
- dna for each dino > traits
