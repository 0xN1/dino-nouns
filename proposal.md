# NSFW: DinoNouns | Interactive On-chain NFT

  ![](https://i.imgur.com/0poFBc9.png)

## TL;DR

- Develop an interactive NFT experience using Nouns assets (Dino head-based Nouns)
- On-chain interactive NFT leveraging `animation_url` in NFT metadata
- On-chain HTML, CSS and JS with option for customization 
- Sandbox for creating a new interactive experience for the Nouns ecosystem
- 2 months of work for refining, adding features, and open-sourcing

## **Ideas** ⌐◨-◨

![](https://i.imgur.com/9xw5iFb.png)

Ohaiii NounsDAO, I'm **Nero One**, an active member from [NounsMY](https://twitter.com/NounsMY)!

I **love to experiment** and **explore different mediums** and NFT, it opens up a new way of doing even more than we could before. 

I've seen some of the stuff people have been doing in the space and it inspires me a lot! But **I saw a lack of creation**/innovation in terms of **interactive** NFT. 


### *The "WHAT IF"*

So I've been thinking, **what if DinoNouns can be interactive** and at the same time the whole thing is all on-chain? What if we can **teach** the character some **words** so it can reply us back? Make it **jump**? Perhaps changing the **DinoTerminal** skins? It would be cool to play with!

Before I continue, here's a quick note on my past projects: 

### *Past Project*

I've **worked on several Interactive NFT projects** and most of it was off-chain, **[COMLINK+](https://opensea.io/assets/ethereum/0x1b7e73c6d30dd5dd811cbd26d9bf36e34882fd39/3)** (pointed to a hosted site), **[tulsv1](https://exchange.art/editions/HkMrXQ7NRZy7UuSvLSpW8Vhut7ZnPn9phRYKerCZ8uba)** (uploaded to IPFS).

### *Fully On-Chain?*

However this time I wanted to **fully put** the **whole HTML on-chain + interactive**.

So to achieve this, **all assets need to be encoded in base64** (**HTML, CSS, JS, fonts**) and to be **included in the smart contract**. Oh and I'm **using vanilla HTML, CSS and JS** to make it simple as possible without any other dependencies.

### *Nouns SVG*

For Nouns SVG generation, I'm currently using **NounsDescriptorV2** contract to generate on-chain SVG for **DinoNouns**. To be used in both of the `image` (in teh metadata) and in the HTML itself.

**Seed** for the generation is based on **Dino name** and **tokenId** of the NFT:

`uint256 pseudorandomness = uint256(keccak256(abi.encodePacked(_name, _id)));`

### *Dynamic NFT?*

Each Dino **name** is **stored on-chain** and to change it, you're required to interact with the DinoNouns contract. **Changing name** will **reroll the Dino** .

Do you want to **re-skin** your **DinoTerminal**? You **can** do it! **Customize your CSS** and **put** that into the **contract**! Oh, it's **token mapped**. So **if you do for your token**, **only u get the custom CSS**!


## **Summary** ⌐◨-◨

![](https://i.imgur.com/OnCIz9S.png)

### Vision

>**The token is the canvas - Nahiko**

To bring awareness on on-chain interactive NFT and how the community can utilise it

### Objective
1. NounsDAO **community can fork**, **experiment** and **play** with their own **idea/interaction** they want to bring into their project.
2. **Opening up new possibilities** for **future Nouns fork** to embed interaction within the project

### Strategy
1. Build HTML-based interaction with UI/UX
2. Create smart contract architecture for the on-chain interaction and utilisation of HTML, JS and CSS.
3. Make use of the existing Nouns ecosystem [`NounsDescriptor` and `NounsSeeder`]
4. Refine the codebase for future fork
5. Open-source it!

## **Deliverables**

![](https://i.imgur.com/MXRtvzs.png)

1. I have built the MVP (minimum viable product) for the project. This includes:
    - UI/UX Design
        - [Figma](https://www.figma.com/file/vQKWi2HJQZjmzmEAAMC1Nm/DinoNouns?node-id=0%3A1)
        ![](https://i.imgur.com/UeikhhP.png)
    - Interactive HTML Page demo deployed on Surge
        - [Demo](https://recondite-flame.surge.sh/)
        ![](https://i.imgur.com/kct6c04.png)
    - Deployed initial prototype  on Goerli Testnet
        - [Goerli DinoNouns](https://goerli.etherscan.io/address/0x1c5c48e2ff4ac1e4849051b41b4ef44998f23277)
        - [Testnet OpenSea](https://testnets.opensea.io/collection/dinonouns)
        - [DinoNoun-0 on Testnet OpenSea](https://testnets.opensea.io/assets/goerli/0x1c5c48e2ff4ac1e4849051b41b4ef44998f23277/0)
        ![](https://i.imgur.com/gHXUKmJ.png)
    - Smart contract architecture
        - [FigJam](https://www.figma.com/file/hgitaUUfdGGwoJcCmBnCsu/Diagram---DinoNouns?node-id=0%3A1)
        ![](https://i.imgur.com/0eQ711j.png)
    - Contract deployment on Mainnet 
        - [DinoNouns](https://etherscan.io/address/0xb43e886c7d7d4b3eda65e016b5bcef56548aeb7b)
        - [DinoRenderer](https://etherscan.io/address/0x4484a56a643dbbe2e074c3ad53d1b8de4ccc604d)
        - [DinoUtility](https://etherscan.io/address/0x56b5288079b6e34ae6a8a5c9cd618fbc9f3d7997)
    - DinoNouns collection on OpenSea and minted 3
        - [DinoNouns OpenSea](https://opensea.io/collection/dinonouns)
        - [DinoNouns-0 on OpenSea](https://opensea.io/assets/ethereum/0xb43e886c7d7d4b3eda65e016b5bcef56548aeb7b/0)
        ![](https://i.imgur.com/vlKL8Q4.png)
    - GitHub repo for the project (work in progress)
        - [dino-nouns](https://github.com/0xN1/dino-nouns)
2. Report and updates will be posted on [my social media](https://twitter.com/0xNeroOne) and discourse.
3. Refine, add features and prepare the repo for open-source
    - [dino-nouns](https://github.com/0xN1/dino-nouns)

### Features
- Text-based command interaction
- Dynamic on-chain name
- CSS Animation
- Utility commands
- Dynamic favicon and title (only if you view it in a separate tab)
- Custom CSS
- Teach your dino wordsssss~
- Commands have a `30%` chance to fail - hehehehe
- Map commands to button :)
- Use keyboard shortcut `[a,b,x,y]` for the buttons
- and more...

### Commands

List of commands

| Command | Desc | Usage | eg |
|-|-|-|-|
|/dino|give temporary nickname|/dino [name]|/dino abu|
|/run|make dino run|/run|/run|
|/jump|make dino jump|/jump|/jump|
|/clear|clear logs|/clear|/clear|
|/reset|reset to default dino|/reset|/reset|
|/map|map command to button|/map [btn][command]|/map a run|
| /teach| teach your dino words!|/teach [word] [reply]| /teach yo whatsupp!|
|/help|help command|/help [command]|/help [cmd]|
|[any]|dino will say it back|[any]|hi|
| nouns | Link to nouns.wtf| nouns | nouns|
| center | Link to nouns.center| center | center|

You can create yours too if you fork the project! :)

## **Budget Breakdown** ⌐◨-◨

![](https://i.imgur.com/eXqtDbk.png)

I'm asking for:

- 6 ETH - Work done for the current MVP on [deliverables](#deliverables)
- 4 ETH - Work done for [deliverables 2 and 3](#deliverables) (December 2022)

Payable to `neroone.eth || 0xA6c0F7bde119930fB919ed02F8155887EcF0D756` 😁

oh ya guysss, please let me know about anything~

![](https://i.imgur.com/T0fcBWJ.png)

Thank you for reading. wohohoooooooo~ 🙏🙏