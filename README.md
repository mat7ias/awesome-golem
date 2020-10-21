# Awesome Golem [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Welcome to **Awesome Golem**, a community-curated list of resources, links, projects, tools and apps on Golem!
Note: this guide and it's contents is specific to New Golem and it's current implementation, Yagna. For Legacy (Clay) Golem, you can find the documentation [here](https://docs.golem.network/) and [comms archive](https://trello.com/b/95eZBUfT/golem-comms-archive).

### Contents

- [Golem](#golem)
  - [Docs](#docs-and-releases)
  - [Explorers](#explorers)
- [Developer Resources](#developer-resources)
  - [Tools](#-tools)
  - [Apps](#%EF%B8%8F-apps)
  - [Testnet NGNT and Ether](#-testnet-ngnt-and-ether)
  - [Bounties and Hackathons](#-bounties-and-hackathons)
- [Running a Golem Node](#running-a-golem-node)
  - [Testnet](#mainnet)
  - [Mainnet](#mainnet)
- [Learning Resources](#learning-resources)
  - [Interesting Links](#-interesting-links)
  - [GitHub Digest](#-GitHub-Digest)
- [Community Incentives Program](#community)
- [Other Resources](#other-resources)

# Golem

- [Website](https://golem.network/)
- [Github](https://github.com/golemfactory)
- [Chat](https://chat.golem.network/)
- [Reddit](https://reddit.com/r/GolemProject)
- [Twitter](https://twitter.com/golemproject)
- [Blog](http://blog.golemproject.net/)

### Docs and releases

- [Yagna handbook](https://handbook.golem.network/)
- [Releases List](https://github.com/golemfactory/yagna/releases)

### Explorers

> Visualization and network statistics of New Golem

- Rinkeby testnet TBD

## Developer Resources

### 👷 Tools

- [Hashcat](https://handbook.golem.network/requestor-tutorials/create-your-own-application-on-golem/the-steps-to-do) - hashcat password-recovery example, this tutorial is designed to inspire you to create your own Golem applications, we will explain all the needed details of Golem application implementation.
- [golem-ortools](https://github.com/Doc-Saintly/golem-ortools) - uses the or-tools Constraint Programming library to solve problems on the golem network.
- [golem-jtr](https://github.com/hhio618/golem-jtr) - run John The Ripper on Golem Nodes to recover a password
- [gvm-vim](https://github.com/canokaue/gvm-vim) - A golemized docker image for compiling the most loved vim editor

### 🖥️ Apps

> Demos, hackathon+bounty app submissions and projects building on/with Golem.

- [golem.network video transcoder](https://golem-video.jarvispowered.com:5000) - This is sample app that uses golem.network to transcode videos. Please select your transcoding profile and then upload your videos.
- [golemGraphWavePair](https://github.com/smiley1983/golemGraphWavePair) - Use the Golem Network to generate graph frames, then combine them into an animation.
- [golemized-strong-gravitational-lense](https://github.com/rezahsnz/golemized-strong-gravitational-lense) - a simple distributed computing hack that tries to simulate some physical phenomena called gravitional lensing and is based on the work of Prof. Adam Bolton.

### 💸 Testnet NGNT and Ether

If for any reason the faucet was unsuccessful, grab some testnet Ether via the [Rinkeby faucet](https://faucet.rinkeby.io/), send it to your node address (can be found with `yagna app-key list`, starts with "0x...") and run the command `yagna payment init -r` again.

If you have the MetaMask browser extension installed you can also try the [MetaMask faucets](https://faucet.metamask.io). Change to Rinkeby test network by clicking at the top on 'Main Ethereum Network' and select Rinkeby.

### 👷 Bounties and Hackathons

> Details on Golem bounties.

Compile VIM On Single Golem Node - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/702/100023963)
 1. https://github.com/canokaue/gvm-vim
 2. https://github.com/rezahsnz/golemized-vim
 3. https://github.com/iRhonin/golem-vim
 4. https://github.com/thomgabriel/golem-compile-VIM
 5. https://github.com/molecula451/gvim

Process And Visualize Interesting Computations In Matplotlib On Multiple Golem Nodes - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/703/100023964)
 1. https://github.com/smiley1983/golemGraphWavePair
 2. https://github.com/rezahsnz/golemized-strong-gravitational-lense

Run John The Ripper On Multiple Golem Nodes To Crack A Password - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/704/100023965)
 1. https://github.com/Doc-Saintly/golem-john-jumbo
 2. https://github.com/rezahsnz/golemized-john
 3. https://github.com/iRhonin/golem-john
 4. https://github.com/hhio618/golem-jtr

Create A Video Transcoding Web Application Using Golem As A Backend - [Gitcoin link](https://gitcoin.co/issue/golemfactory/yagna/705/100023966):
 1. https://github.com/Doc-Saintly/golem-video

## Running a node on New Golem

### Testnet

#### Requestor:
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

#### Provider:
https://handbook.golem.network/provider-tutorials/provider-tutorial

1. Installation: `curl -sSf https://join.golem.network/as-provider | bash -`
2. Start the Golem Sneak Peak provider release: `golemsp run`

### Mainnet

[New Golem is not yet on mainnet. This section will be updated after MVP launch.]


## Learning Resources

- [Unraveling Golem’s The Next Milestone](https://blog.golemproject.net/next-milestone)
- [Unraveling Golem’s The Next Milestone, Part II](https://blog.golemproject.net/next-milestone-part-ii/)
- [Unraveling Golem’s The Next Milestone, Part III](https://blog.golemproject.net/next-milestone-part-iii/)

### 🔖 Interesting Links

- [Golem Legacy FAQ](https://docs.golem.network/#/About/FAQ)
- [Golem Telegram resources bot (contains information only)](https://t.me/GolemInfoBot)

### Videos and presentations

- [Golem Loves Layer 2 presentations and panel](https://youtu.be/B8Qu-Nofbaw) - 
- [New Golem - Alpha 2 Release - Quick intro](https://youtu.be/TenOjOql5vA) - Kuba
- [New Golem - Alpha II Requestor Primer Tutorial](https://youtu.be/UHL-5QfoWmo) - Mattias
- [EDCON - Building New Golem: Where We're at and Where We're Heading](https://www.youtube.com/watch?v=FVzn1G9wtUg&feature=youtu.be&t=901) - Kuba
- [ReadyLayerOne - A Golem (R)evolution](https://youtu.be/s9WdFqLyLFo) - Piotr Janiuk


### 📝 GitHub Digest

- [Golem GitHub Digest #1](https://blog.golemproject.net/golem-github-digest-1/)
- [Golem GitHub Digest #2](https://blog.golemproject.net/golem-github-digest-2/)
- [Golem GitHub Digest #3](https://blog.golemproject.net/golem-github-digest-3/)
- [Golem GitHub Digest #4](https://blog.golemproject.net/golem-github-digest-4/)
- [Golem GitHub Digest #5](https://blog.golemproject.net/golem-github-digest-5/)
- [Golem GitHub Digest #6](https://blog.golemproject.net/golem-github-digest-6/)
- [Golem GitHub Digest #7](https://blog.golemproject.net/golem-github-digest-7/)

## Community

[Golem Community Incentives Program](https://blog.golemproject.net/community-incentives-program/) - Participate in the community and get rewarded for it in GNT!

## Other Resources

