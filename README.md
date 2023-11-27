<p align="center"><img width="500" src="./assests/Logo3.png"></p>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/Platform-Telegram-blue)](https://desktop.telegram.org/)
![GitHub](https://img.shields.io/badge/Language-Python-blue.svg)
[![GitHub contributors](https://img.shields.io/github/contributors/sak007/MyDollarBot-BOTGo)](https://github.com/ebanigogia/dollar_bot/graphs/contributors)
[![DOI](https://zenodo.org/badge/706356133.svg)](https://zenodo.org/doi/10.5281/zenodo.10019963)
[![Build Status](https://app.travis-ci.com/usmanwardag/dollar_bot.svg?branch=main)](https://app.travis-ci.com/usmanwardag/dollar_bot)
[![codecov](https://codecov.io/gh/usmanwardag/dollar_bot/branch/main/graph/badge.svg?token=PYAWX95R67)](https://codecov.io/gh/usmanwardag/dollar_bot)

[![GitHub issues](https://img.shields.io/github/issues/ameghana/CSC510-FALL23-P27-Project3-dollar_bot)](https://github.com/ameghana/CSC510-FALL23-P27-Project3-dollar_bot/issues)
[![GitHub closed issues](https://img.shields.io/github/issues-closed/ameghana/CSC510-FALL23-P27-Project3-dollar_bot)](https://github.com/ameghana/CSC510-FALL23-P27-Project3-dollar_bot/issues?q=is%3Aissue+is%3Aclosed)
[![GitHub pull requests](https://img.shields.io/github/issues-pr/ameghana/CSC510-FALL23-P27-Project3-dollar_bot)](https://github.com/ameghana/CSC510-FALL23-P27-Project3-dollar_bot/pulls)
[![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
[![GitHub Discussions](https://img.shields.io/github/discussions/ameghana/CSC510-FALL23-P27-Project3-dollar_bot)](https://github.com/ameghana/CSC510-FALL23-P27-Project3-dollar_bot/discussions)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
[![Discord](https://img.shields.io/discord/1161405668079698112)](https://github.com/ameghana/CSC510-FALL23-P27-Project2/blob/main/docs/SE%20Discord%20Chat%20Screenshot.png)
![GitHub forks](https://img.shields.io/github/forks/ameghana/CSC510-FALL23-P27-Project3-dollar_bot)


<hr>
<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#why-should-you-use-dollar-bot">Why should you use Dollar Bot?</a></li>
    <li><a href="#check-out-the-video">Check out the video!</a></li>
    <li><a href="#what-is-new-in-this-version">What is new in this version?</a></li>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#testing">Testing</a></li>
    <li><a href="#code-coverage">Code Coverage</a></li>
    <li><a href="#License">License</a></li>
    <li><a href="#code-documentation">Code Documentation</a></li>
    <li><a href="#how-to-contribute">How to Contribute</a></li>
    <li><a href="#future-roadmap">Future RoadMap</a></li>
   <li><a href="#contributors">Contributors</a></li>
   <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

<hr>

## Why should you use MyDollar Bot?

Dollar Bot is an easy-to-use Telegram Bot that assists you in recording your daily expenses on a local system without any hassle.  
With simple commands, this bot allows you to:
- Add/Record new spendings
- Display your spendings through bar graph
- Show the sum of your expenditure for the current day/month
- Display your spending history
- Clear/Erase all your records
- Edit/Change any spending details if you wish to

## Check out the video!

[![Demo Video](https://i9.ytimg.com/vi/aCjcT1CHAzU/mq3.jpg?sqp=COSotI0G&rs=AOn4CLD34jFIlq6GRdmTnK6p3F8O2F-Yig)](https://www.youtube.com/watch?v=O0sEIM39ejE)

## What is new in this version?

Checkout the [this documentation](https://github.com/ebanigogia/dollar_bot/blob/main/What_is_new.pdf)
## Installation

The below instructions can be followed in order to set-up this bot at your end in a span of few minutes! Let's get started:

1. Clone this repository to your local system.

2. Start a terminal session in the directory where the project has been cloned. Run the following command to install the required dependencies:
```
  pip install -r requirements.txt

```
3. Download and install the Telegram desktop application for your system from the following site:
 ```
 https://desktop.telegram.org/
 ```
## How to run?

1. In Telegram, search for "BotFather". Click on "Start", and enter the following command:
```
  /newbot
```
2. Follow the instructions on screen and choose a name for your bot (e.g., `dollarbot`). After this, select a username for your bot that ends with "bot". The username has to be unique. 

3. BotFather will now confirm the creation of your bot and provide a TOKEN to access the HTTP API - copy and save this token for future use.

4. In the repo directory (where you cloned it), run these commands to (i) grant execution access to a bash script, and (ii) execute that bash script to run the Telegram Bot:
```
   chmod a+x run.sh
   ./run.sh
```
   
(OR)
```
   chmod a+x run.sh
   bash run.sh
```
```Note```: It will ask you to paste the API token you received from Telegram in step 4.
A successful run will generate a message on your terminal that says "TeleBot: Started polling." 

5. In the Telegram app, search for your newly created bot by entering the username and open the same. Now, on Telegram, enter the "/start" or "menu" command, and you are all set to track your expenses!

### Run Automatically at Startup

To run the script automatically at startup / reboot, simply add the `.run_forever.sh` script to your `.bashrc` file, which executes whenever you reboot your system.

## Testing

We use pytest to perform testing on all unit tests together. The command needs to be run from the home directory of the project. The command is:
```
python run -m pytest test/
```

## Code Coverage

Code coverage is part of the build. Every time new code is pushed to the repository, the build is run, and along with it, code coverage is computed. This can be viewed by selecting the build, and then choosing the codecov pop-up on hover.

Locally, we use the coverage package in python for code coverage. The commands to check code coverage in python are as follows:

```
coverage run -m pytest test/
coverage report
```

## License

This project is licensed under the terms of the MIT license. Please check [License](https://github.com/usmanwardag/dollar_bot/blob/main/LICENSE) for more details.


## Code Documentation

Checkout the [docs](https://github.com/sak007/MyDollarBot-BOTGo/tree/main/docs)

## How to Contribute

We would be happy to receive contributions! If you'd like to, please go through our [CONTRIBUTING.md](https://github.com/usmanwardag/dollar_bot/blob/main/CONTRIBUTING.md)

For any feedback, issues, or bug reports, please create an issue [here](https://github.com/usmanwardag/dollar_bot/issues/new).

## Future RoadMap

- More content can be added for the way notifications can be displayed on the user front. This can be done to make the UI more interactive.
- Recurring expenses feature can be added for faster addition of expenses instead of following the whole process of everytime.

## Contributors
<table>
  <tr>
    <td align="center"><a href="https://github.com/ebanigogia"><br /><sub><b>Ebani Gogia</b></sub></a></td>
    <td align="center"><a href="https://github.com/shrishty19"><br /><sub><b>Shrishty Singh</b></sub></a><br /></td>
    <td align="center"><a href="https://github.com/rhythmjagota"><br /><sub><b>Rhythm Jagota</b></sub></a><br /></td>
  </tr>
</table>

## Chat Channel

- https://discord.com/channels/1164337248746082394/1164337249387823152

## Acknowledgements

- We would like to express our gratitude 🙏🏻 and a big thank you 😇 to Prof. Dr. Timothy Menzie for giving us the opportunity to get into the shoes of software building and learning new skills and development process throught the project building.
- A big thank you 😊 to the Teaching Assistants for their support.
- Thank you to the previous team 😊 for a thorough ReadMe and deatiled documentation.[MyDollarBot](https://github.com/sak007/MyDollarBot-BOTGo)
- Thank you to the ⭐️[Telegram bot](https://github.com/python-telegram-bot/python-telegram-bot)




