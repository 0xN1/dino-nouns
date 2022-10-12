# **Progress and content dump**

- Deployed html renderer contract 
    - [Test on Goerli](https://goerli.etherscan.io/address/0x8192F63E9F21E7e0D844a4abCF471D59A91553Fb#code)

- First initial prototype HTML
    - uses [CloudNouns API](https://docs.cloudnouns.com) for SVG generation

    - ![](https://cdn.discordapp.com/attachments/1014135287087108196/1026983796152746004/unknown.png)

- [Link to twitter video](https://twitter.com/0xNeroOne/status/1577246189732315136?s=20&t=INjXxBacD6JgeaU-3u8suQ)

    - ![](https://cdn.discordapp.com/attachments/1014135287087108196/1029638192011427861/unknown.png)

- started working on a mockup design
    - [Figma](https://www.figma.com/file/vQKWi2HJQZjmzmEAAMC1Nm/DinoNouns?node-id=0%3A1)
    
    - ![](https://i.imgur.com/UeikhhP.png)
    
    - ![](https://media.discordapp.net/attachments/1014135287087108196/1028490039811903579/unknown.png)
- translated most some of the design to code
- deployed to surge for testing 
    - [demo](https://recondite-flame.surge.sh/)
- added map cmd, so u can map the button to command. so no need retype every time :)
- tried deploying the renderer contract for dinonouns
- doesn't work because of localStorage blocked on opensea
- removed the localStorage, so no state saving for the dino, it works now
    - [testnet 1](https://testnets.opensea.io/assets/goerli/0x3b9ba7ea888051376e5f5d7a0a68d167bfea4b05/1)
- deployed new NFT contract on goerli
    - [testnet 2](https://testnets.opensea.io/assets/goerli/0x1c5c48e2ff4ac1e4849051b41b4ef44998f23277/0)
- added on-chain dino name
- token owner can use `setDinoName(string,uint)` to change their dino name on the contract.
- added custom CSS feature. here are some of the test.
    - ![](https://cdn.discordapp.com/attachments/1014135287087108196/1029313032133804102/unknown.png)
    - ![](https://cdn.discordapp.com/attachments/1014135287087108196/1029313069412794368/unknown.png)
    - ![](https://cdn.discordapp.com/attachments/1014135287087108196/1029313069412794368/unknown.png)
- token owner can use `setCustomCSS(string,uint)` to add custom CSS for their dinoTerminal.
    - eg: `"*{color:red}"` - will set the text to red
- deployed contract to mainnet
     - [DinoNouns](https://etherscan.io/address/0xb43e886c7d7d4b3eda65e016b5bcef56548aeb7b)
    - [DinoRenderer](https://etherscan.io/address/0x4484a56a643dbbe2e074c3ad53d1b8de4ccc604d)
    - [DinoUtility](https://etherscan.io/address/0x56b5288079b6e34ae6a8a5c9cd618fbc9f3d7997)
- Minted 3 NFT from the DinoNouns collection so that community could play with it. 
    - [DinoNouns OpenSea](https://opensea.io/collection/dinonouns)
    - ![](https://i.imgur.com/vlKL8Q4.png)
- made a proposal  in NounsDAO Small Grants discourse 😆
