# Predicting-FIFA-23-Ultimate-Team-Player-Market-Prices

![FUT PICTURE](./Images/FUT-23-Event-Promo-Release.png)

# Background

### What is FIFA Ultimate Team?

FIFA Ultimate Team (FUT) is a popular game mode within the FIFA video game franchise that allows players to build their own virtual football team by collecting and trading player cards. Each player card has its own set of attributes and can be used in matches against other players' teams. Player cards in FIFA Ultimate team can be obatined in a variety of ways such as through packs, the transfer market, rewards, and special events. Each method has its own advantages and disadvantages, and the best method may depend on the player's preferences, budget, or playing style. Each player card in the game has an overall rating, face card ratings (PAC, DRI, PAS, DEF, PHY, SHO) as well as in-game stats which are all meant to closely reflect their real life ability in matches. 


# Business Problem

![Alt](./Images/corporate-meeting-with-finance-director.jpg)

This project will mainly focus on players obtaining player cards through the transfer market and how player card prices are determined. Naturally we would believe that the higher the rating the higher the market price. However, there are many situations where this is not the case and so the aim of this project is to explore which factors are most important when determing a players market price value and in doing so create a suitable machine learning  model using FIFA 23 Ultimate data to predict player card prices.

# Obtaining the Data and Data Cleaning

## Where did the data come from?

The dataset was downloaded from Kaggle and the creator was Lucas Silva. The data was scraped from the Futbin a famous FIFA Ultimate Team site that contains the database from all Ultimate Team players and features.


Below is an overview of all the features included in the dataset and which will be considered when creating the Machine Learning model:

Name = Name of player

Club = Club that player plays for

Nation = Players nation

League = League that club is in

Rating = Players overall rating 0-99

Main_postion = Positon that is on the face of that players card

Alternate_Positions: the positions that the player can also play

Card_Version: type of the card - Rare Gold, ICON, Common Gold

Run_Style: the way player runs - Explosive, Controlled and Lenghty

Price: the current price of the player on Ultimate Team Market

Price_Variation: the daily price difference

Skills_Star: measures how many skills a player can do - varies from 1 to 5

WeakFoot_Star: measures how well a player execute actions with his weak foot - varies from 1 to 5

Attack_Workrate: measures how is the intensity of the player attacking - High, Medium and Low

Defense_Workrate: measures how is the intensity of the player defending - High, Medium and Low

Pace / Diving: Pace: how fast a player is in game / Diving: how well a goalkeeper jumps to the ball - 0 to 99

Shooting / Handling: Shooting: how well a player shoots in game / Handling: how well a goalkeeper is with his hands - 0 to 99

Passing / Kicking: Passing: how well a player pass in game / Kicking: how well a goalkeeper kicks the ball - 0 to 99

Dribbling / Reflexes: Dribbling: how well a player dribbles in game / Reflexes: how fast a goalkeeper reacts to the ball - 0 to 99

Defense / Speed: Defense: how well a player defends in game / Speed: how fast a goalkeeper is in game- 0 to 99

Physical / Positioning: Physical: how strong a player is in game / Positioning: how well a goalkeeper positionates himself in goal - 0 to 99

Height: in centimeters / in feet

BodyType: how is the player's body in game

Popularity: the balance of likes and dislikes in the Futbin

Base_Stats: the sum of the stats from the front of card

Ingame_Stats: the sum of all stats from the player


## Dealing with player cards with a price of '0'







