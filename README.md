# Awesome Golem [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Welcome to **Awesome Golem**, a community-curated list of resources, links, projects, tools and apps on Golem!
Note: this guide and it's contents is specific to New Golem and it's current implementation, Yagna. For Legacy (Clay) Golem, you can find the documentation [here](https://docs.golem.network/) and [comms archive](https://trello.com/b/95eZBUfT/golem-comms-archive).

### Contents

- [Golem](#golem)
- [Apps](#%EF%B8%8F-apps)
  - [Tools](#tools)
  - [Bounties and Hackathons](#bounties-and-hackathons)
- [Developer Resources](#-developer-resources)
  - [Docs and Releases](#docs-and-releases)
  - [Running a node on New Golem](#running-a-node-on-new-golem)
  - [Testnet NGNT and Ether](#testnet-ngnt-and-ether)
- [Learning Resources](#learning-resources)
  - [Unraveling Golem’s The Next Milestone series](#unraveling-golems-the-next-milestone-series)
  - [Videos and presentations](#videos-and-presentations)
  - [GitHub Digest](#gitHub-digest)
- [Community Incentives Program](#community)

# Golem

- [Golem.Network Website](https://golem.network/) - The official Golem Network website.
- [Golem Factory Github](https://github.com/golemfactory) - Where you can find the open source code of all things Golem!
- [Golem Community Chat](https://chat.golem.network/) - Join the community and team open discussion on Discord.
- [Reddit](https://reddit.com/r/GolemProject) - Golem Network discussion on the Reddit platform.
- [Twitter](https://twitter.com/golemproject) - The Golem Project Twitter.
- [Blog](http://blog.golemproject.net/) - The official blog where you can find the most reliable information on announcements, summaries and updates.

# 🖥️ Apps

> Demos, hackathon+bounty app submissions and projects building on/with Golem.

- [golem.network video transcoder](https://golem-video.jarvispowered.com:5000) - This is sample app that uses golem.network to transcode videos. Please select your transcoding profile and then upload your videos.
- [Hashcat](https://handbook.golem.network/requestor-tutorials/create-your-own-application-on-golem/the-steps-to-do) - hashcat password-recovery example, this tutorial is designed to inspire you to create your own Golem applications, we will explain all the needed details of Golem application implementation.
- [golemGraphWavePair](https://github.com/smiley1983/golemGraphWavePair) - Use the Golem Network to generate graph frames, then combine them into an animation.
- [golemized-strong-gravitational-lense](https://github.com/rezahsnz/golemized-strong-gravitational-lense) - a simple distributed computing hack that tries to simulate some physical phenomena called gravitional lensing and is based on the work of Prof. Adam Bolton.
- [golem-parallel-matplotlib](https://github.com/CoeJoder/golem-parallel-matplotlib) - various statistical analyses are performed on circadian rhythm measurements in human test subjects.
- [golem-covid](https://github.com/iRhonin/golem-covid) - This program get a parameter from data/owid-covid-data.csv file (like new_cases_per_million) and plot every day data on the world map. After all images generated (in outputs), it will gather them and create a gif ([example](https://github.com/iRhonin/golem-covid/raw/main/covid.gif?raw=true)).

## Tools

- [golem-ortools](https://github.com/Doc-Saintly/golem-ortools) - uses the or-tools Constraint Programming library to solve problems on the golem network.
- [golem-jtr](https://github.com/hhio618/golem-jtr) - run John The Ripper on Golem Nodes to recover a password.
- [gvm-vim](https://github.com/canokaue/gvm-vim) - A golemized docker image for compiling the most loved vim editor.

## Bounties and Hackathons

> Details on Golem bounties and their submissions.

Compile VIM On Single Golem Node - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/702/100023963)
 1. https://github.com/canokaue/gvm-vim - [[Demo](https://www.youtube.com/watch?v=_Of5vnffJJ0&)]
 2. https://github.com/rezahsnz/golemized-vim - [[Demo](https://youtu.be/ougeYENjLbs)]
 3. https://github.com/iRhonin/golem-vim - [[Demo](https://youtu.be/3FBqp2IiP2E)]
 4. https://github.com/thomgabriel/golem-compile-VIM - [[Demo](https://www.youtube.com/watch?v=jwXyiccyaWE)]
 5. https://github.com/molecula451/gvim - [[Demo](https://github.com/molecula451/gvim#building-docker-image)]

Process And Visualize Interesting Computations In Matplotlib On Multiple Golem Nodes - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/703/100023964)
 1. https://github.com/smiley1983/golemGraphWavePair - [[Demo](https://youtu.be/h_MQKBRYTPw)]
 2. https://github.com/rezahsnz/golemized-strong-gravitational-lense - [[Demo](https://youtu.be/IQ0Xz0PEWoY)]
 3. https://github.com/CoeJoder/golem-parallel-matplotlib - [[Demo](https://youtu.be/hflrBq2OXwA)]
 4. https://github.com/iRhonin/golem-covid - [[Demo](https://www.youtube.com/watch?v=9mgdz6I9xHM])]

Run John The Ripper On Multiple Golem Nodes To Crack A Password - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/704/100023965)
 1. https://github.com/rezahsnz/golemized-john - [[Demo](https://youtu.be/L1ht9E93I_0)]
 2. https://github.com/Doc-Saintly/golem-john-jumbo - [[Demo](https://discord.com/channels/684703559954333727/756161015493951600/766647702514958366)]
 3. https://github.com/iRhonin/golem-john - [[Demo](https://youtu.be/fgBIoS9t158)]
 4. https://github.com/hhio618/golem-jtr - [[Demo](https://youtu.be/d6UIb0i9ePI)]

Create A Video Transcoding Web Application Using Golem As A Backend - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/705/100023966)
 1. https://github.com/Doc-Saintly/golem-video - [[Demo](https://golem-video.jarvispowered.com:5000/static/demo.mkv)]

# 👷 Developer Resources

### Docs and releases

- [Yagna handbook](https://handbook.golem.network/) - Handbook for the New Golem implementation, Yanga.
- [Releases List](https://github.com/golemfactory/yagna/releases) - Github releases of Yagna.

## Running a node on New Golem
> New Golem is currently running on on Rinkeby testnet.

### Requestor:
- Get started quick and make your first request with our [flash tutorial](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development). Make sure you meet the requirements then:
  1. Quick install `curl -sSf https://join.golem.network/as-requestor | bash -`
  2. Eun the daemon `yagna service run`
  3. (Separate shell/terminal) generate and save your app key `yagna app-key create requestor`
  4. enable the daemon as a requestor `yagna payment init -r`
That's it! You're now able to request tasks on the Golem network!

- Running an example:
  - Get your environment setup, install dependencies, download examples and run your first task on the network
   5. `python3 -m venv ~/.envs/yagna-python-tutorial`
   6. `source ~/.envs/yagna-python-tutorial/bin/activate`
   7. `pip3 install -U pip`
   8. `pip3 install certifi yapapi`
   9. `git clone https://github.com/golemfactory/yapapi.git`
   10. `cd yapapi`
   11. `git checkout b0.3`
   12. `export YAGNA_APPKEY=insert-your-32-char-app-key-here` (remember your saved app-key?)
   13. `cd examples/blender`
   14. `python3 blender.py --subnet-tag devnet-alpha.2`

### Provider:
Follow the [Provider section](https://handbook.golem.network/provider-tutorials/provider-tutorial) of our handbook, below are the quick install instructions if you meet the prerequisites (Ubuntu 18.04 and 20.04 with Intel CPU): 

1. Installation: `curl -sSf https://join.golem.network/as-provider | bash -` after which you'll see our [start animation](https://user-images.githubusercontent.com/35585644/96857058-d7817900-145e-11eb-9d02-69614d6f8a29.gif).
2. Start the Golem Sneak Peak provider release: `golemsp run`
3. DONE! Your node should now be running. Check your node's status with `golemsp status`

## Testnet NGNT and Ether

If for any reason the faucet was unsuccessful, grab some testnet Ether via the [Rinkeby faucet](https://faucet.rinkeby.io/), send it to your node address (can be found with `yagna app-key list`, starts with "0x...") and run the payment setup command again `yagna payment init -r`.

If you have the MetaMask browser extension installed you can also try the [MetaMask faucets](https://faucet.metamask.io). Change to Rinkeby test network by clicking at the top on 'Main Ethereum Network' and select Rinkeby.

# 📝 Learning Resources

### Unraveling Golem’s The Next Milestone series

- [Unraveling Golem’s The Next Milestone](https://blog.golemproject.net/next-milestone)
- [Unraveling Golem’s The Next Milestone, Part II](https://blog.golemproject.net/next-milestone-part-ii/)
- [Unraveling Golem’s The Next Milestone, Part III](https://blog.golemproject.net/next-milestone-part-iii/)


### Videos and presentations

- [Golem Loves Layer 2 presentations and panel](https://youtu.be/B8Qu-Nofbaw) - Kuba & Mikolaj (Golem) + Panel: Jay Zhou (Loopring Protocol), Kasima Tharnpipitchai (OMG Network), Alex Gluchowski (MatterLabs), Kelvin Fichter (Optimism), Kuba Kucharski (Golem)
- [New Golem - Alpha 2 Release - Quick intro](https://youtu.be/TenOjOql5vA) - Kuba
- [New Golem - Alpha II Requestor Primer Tutorial](https://youtu.be/UHL-5QfoWmo) - Mattias
- [EDCON - Building New Golem: Where We're at and Where We're Heading](https://www.youtube.com/watch?v=FVzn1G9wtUg&feature=youtu.be&t=901) - Kuba
- [ReadyLayerOne - A Golem (R)evolution](https://youtu.be/s9WdFqLyLFo) - Piotr Janiuk


### GitHub Digest

- [Golem GitHub Digest #1](https://blog.golemproject.net/golem-github-digest-1/)
- [Golem GitHub Digest #2](https://blog.golemproject.net/golem-github-digest-2/)
- [Golem GitHub Digest #3](https://blog.golemproject.net/golem-github-digest-3/)
- [Golem GitHub Digest #4](https://blog.golemproject.net/golem-github-digest-4/)
- [Golem GitHub Digest #5](https://blog.golemproject.net/golem-github-digest-5/)
- [Golem GitHub Digest #6](https://blog.golemproject.net/golem-github-digest-6/)
- [Golem GitHub Digest #7](https://blog.golemproject.net/golem-github-digest-7/)

## Community

[Golem Community Incentives Program](https://blog.golemproject.net/community-incentives-program/) - Participate in the community and get rewarded for it in GNT!
