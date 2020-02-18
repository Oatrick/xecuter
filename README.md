# Xecuter

Xecuter is a machine learning-enabled cryptocurrency trading and backtesting platform that connects to popular cryptocurrency exchanges. Xecuter is written in [TypeScript](https://www.typescriptlang.org/), runs on [Node.js](http://nodejs.org), and utilizes [Tensoflow.js](https://www.tensorflow.org/js).

[Xecuter.io](https://www.Xecuter.io) provides a sleek user interface, premium plugins, and other useful tools combined in to unified trading platform which can be leveraged to improve your trade executions, record keeping, and performance analytics. The Xecuter platform leverages the Hedera Network to provide auditable records in addition and verifiable execution of trades 

[Xecuter.io](https://www.Xecuter.io) platform provides rich intergation with traditional social media and our premium members only social media platform. Only at [Xecuter.io](https://www.Xecuter.io), premium members may choose to use to compete againest eachother in public or private trustless competitions basied on any trading meterics.

*Use Xecuter at your own risk.*

## Details

| Feature 	| Details 	|
|:-------------------------------:	|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------:	|
| Automated trading 	| Default support of basic technical analysis indicators of which <br>the settings of the these indicators may be changed 	|
| Backtesting 	| Monitor live market or import historical market data to<br>perform backtesting, otherwise referred to as paper trading, to<br>access viability of trading strategies 	|
| Broadcast Trade and Market Data 	| Default broadcasting support provided for Twitter, StockTwits,<br>pubsub messaging systems, and the Arweave network 	|
| Support Programmable Strategies 	| Supports ability to create plugins that preforms programmable<br>trading behavior and analysis programmed in javascript 	|

Market data, either live or historical, can be feed in from any supported source, including multiple feeds if desired, and then manipulated as desired for both analysis and decision making purposes.

Xecuter also provides support for tensorflow.js within the programatic strageties to both fine tune settings and identify possible technical suggestions to improve a stragtegies preformace based on desired outcomes. 

## Documentation

Please refer to [documents section](https://docs.xecuter.io#xecuter) on Xecuter's offical site [Xecuter.io](https://www.xecuter.io).

## Installation & Usage

Please refer to [installation section](https://docs.xecuter.io#installation) on Xecuter's offical site [Xecuter.io](https://www.xecuter.io) for guided installation solutions.

***Adanced:*** <br>
**Manunal installation, including the use [Terraform Could](https://www.terraform.io/) , of Xecuter and HederaXecuter using provided Terraform profile is an advanced task and should be throughly tested, by preforming a diagnostics on technical analysis systems with the defualt bot, before depositing funds or deploying on live networks.**

The Xecuter platform can be easily deloyed to any cloud computing service provider using the Terraform profile which can be found in this repository. [Terraform Could](https://www.terraform.io/) can be used simply in a few clicks by forking this repository and your fork of this repository to Terraform Cloud. 

The defualt profile provided has Hedera services bybassed as they require a sperate service, [HederaXecuter (Repository)](https://github.com/Oatrick/HederaXecuter), to intereact with the [Hedera](https://www.hedera.com/). The inital setup using [Terraform Could](https://www.terraform.io/) is same for HederaXecuter, but are additional steps so please review the instructions on setting up Xecuter with HederaXecuter to interact with [Hedera](https://www.hedera.com/) on [Xecuter.io](https://www.Xecuter.com)'s [HederaXecuter installation section](https://docs.xecuter.io#installation#hederaxecuter).

If you would like to learn to build your own payment and messaging server to interact with Xecuter, or any other [Hedera](https://www.hedera.com/) use case, please go to [Hedera](https://www.hedera.com/)'s [documentation resources](https://docs.hedera.com/guides/docs/mirror-node-api/hedera-consensus-service-api-1).**

***Highly Adanced:*** <br>
Installing this repository from source requires knowledge of typescript, compiler tools, [docker](http://www.docker.io), and [Terraform](https://www.terraform.io/), a universial cloud delpoyment standard, or any other prefered cloud computing service provider's deployment tools.

**This method of installation of Xecuter and HederaXecuter is a highly advanced task and should be incredibly throughly tested before used before depositing funds or deploying on live networks. With this installation method, there is an extra step of testing that is highly suggested; This additional test ensures Xecuter's machine learning functions, its ablity to connect to a functioning Bitcoin network, create wallets, receive, send bitcoin transactions, ensures that the trading analysis performs as expected, and most importantly this test determins, in a closed system that, Xecuter can properly recognize internal changes from external sources to it's internal dataset; this final check is ensure that Xecuter will not get confused by multiple identical Xecuter bots making identical choices running on the same Xecuter instance.**

**Installing from source:**

Step One: Clone this repository

Step Two: ...

**After installing and running the technical analysis diagnostic on Xecuter, please preform the following diagnostic test with only a single default bot running:**

Step One: Delpoy a local Bitcoin testnet

Step Two: Mine at least 101 blocks

Step Three: Open the console and enter the command: `Xecuter -reset --selfplay=on`

**Note:** This resets Xecuter in selfplay mode which spans an additional instance of the bot. This tests both the ML functions of Xecuter at the sametime as its ablity to connect to a functioning Bitcoin network, create wallets, receive, and send bitcoin transactions.

Step Three: Follow the prompt's instructions to connect to the local Bitcoin testnet 

Step Five: When prompt with the twin's public keys send exactly 10 BTC into each of their addresses

Step Six: Mine atleast 11 more blocks

Step Seven: Open the console and enter the command `Xecuter -train --dataset=default --max-ganuality=1h --log=all` 

**Note:** The above command will have both Xecuters train in the same enviorment, which they are both changing, and they will only make decisions considering 1h timeframe or higher; setting to a lower timeframe setting will make the simulation take much longer and require much more stroage space to store the results. This test uses default dataset which is full price data from the BTCUSD on Bitstamp exchange from 2016 to 2018.

Step Eight: Wait until training is complete... this may take up to two hours on slower computers

**Note:** If it is taking longer force close the program, then wipe the chache and repeat Steps Three through Six; at Step Seven, instead of setting `--max-ganuality=1h` set it to `--max-ganuality=4h`. This should reduce the the wait time, but if it still takes too long then there is software or hardware issue not related to Xecuter.

Step Nine: When prompted to compare results select `Default SelfPlay Baseline Resluts` then a new five paned window will open in an indepth analysis of each of the four bots, the two bots from your test and the two from the baseline, and the fifth pane is for of the results compairison. In the compairison pane, there is a diffrence figure in red and if it is under 2% then your test and installation was successful!😌

## Community & Support

For the latest news and annonucments, follow [@Xecuter_IO](https://twitter.com/Xecuter_IO) on Twitter.

Xecuter has a [subreddit (r/Xecuter)](https://www.reddit.com/r/Xecuter/) and a [telegram channel](https://t.me/xecuteroffical) for discussions about Xecuter, automated trading, machine learning in trading, technical analysis and exchanges. 

Xecuter has a informational and educational [youtube channel](https://www.youtube.com/channel/UCmvFJnLpX9MgiNfgGy3_iFQ/featured) which has turorials and community content.

Email: xecuter_io (AT) protonmail.com

## Special Thanks

To the IndieHacker community and the developer [AskMike](https://github.com/askmike) who developed Gekko which Xecuter was orginally based on.

More information on Gekko can be found here: 
[Article](https://medium.com/@gekkoplus/archiving-open-source-gekko-dba02e6efc7), [Repository](https://github.com/askmike/gekko)

![Gordon Gekko](http://mikevanrossum.nl/static/gekko.jpg)

*The most valuable commodity I know of is information.*

-Gordon Gekko

Tip Bitcoin to [AskMike](https://github.com/askmike): 13r1jyivitShUiv9FJvjLH7Nh1ZZptumwW
