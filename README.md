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

### 🖥️ Apps

> Demos, hackathon+bounty submissions and projects building on/with Golem.

- [golem-ortools](https://github.com/Doc-Saintly/golem-ortools) - uses the or-tools Constraint Programming library to solve problems on the golem network.
- [golem-john-jumbo](https://github.com/Doc-Saintly/golem-john-jumbo) - a sample program that uses golem.network to run John the Ripper -Jumbo to break an md5 password hash.

### 💸 Testnet NGNT and Ether

If for any reason the faucet was unsuccessful, grab some testnet Ether via the [Rinkeby faucet](https://faucet.rinkeby.io/), send it to your node address (can be found with `yagna app-key list`, starts with "0x...") and run the command `yagna payment init -r` again.

If you have the MetaMask browser extension installed you can also try the [MetaMask faucets](https://faucet.metamask.io). Change to Rinkeby test network by clicking at the top on 'Main Ethereum Network' and select Rinkeby.

### 👷 Bounties and Hackathons

> Details on Golem bounties.

- [Compile VIM On Single Golem Node](https://gitcoin.co/issue/golemfactory/yagna/702/100023963)
- [Process And Visualize Interesting Computations In Matplotlib On Multiple Golem Nodes](https://gitcoin.co/issue/golemfactory/yagna/703/100023964)
- [Run John The Ripper On Multiple Golem Nodes To Crack A Password](https://gitcoin.co/issue/golemfactory/yagna/704/100023965)
- [Create A Video Transcoding Web Application Using Golem As A Backend](https://gitcoin.co/issue/golemfactory/yagna/705/100023966)


## Running a node on New Golem

### Testnet

#### Requestor:
- Get started quick and make your first request with our [flash tutorial](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development). Make sure you meet the requirements then:
  - quick install `curl -sSf https://join.golem.network/as-requestor | bash -`
  - run the daemon `yagna service run`
  - (separate shell/terminal) generate and save your app key `yagna app-key create requestor`
  - enable the daemon as a requestor `yagna payment init -r`
That's it! You're now able to request tasks on the Golem network!

- Running an example:
  - Get your environment setup, install dependencies, download examples and run your first task on the network
   - `python3 -m venv ~/.envs/yagna-python-tutorial`
   - `source ~/.envs/yagna-python-tutorial/bin/activate`
   - `pip3 install -U pip`
   - `pip3 install certifi yapapi`
   - `git clone https://github.com/golemfactory/yapapi.git`
   - `cd yapapi`
   - `git checkout b0.3`
   - `export YAGNA_APPKEY=insert-your-32-char-app-key-here` (remember your saved app-key?)
   - `cd examples/blender`
   - `python3 blender.py --subnet-tag devnet-alpha.2`

#### Provider:
- Regular installation: `curl -sSf https://join.golem.network/as-provider | bash -`
OR
- Dev installation: `curl -sSf https://join.golem.network/dev/as-provider | bash -`

Start the Golem Sneak Peak provider release with `golemsp run`

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

