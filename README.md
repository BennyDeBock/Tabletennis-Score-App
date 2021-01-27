# Tabletennis-Score-App
A rewrite of the original Table Tennis score appllication in C# with added features


# Purpose of this App
The original purpose of the app was a way to easily print match sheets for our club.
The app I'm developing will be converting visual basic to C# for easier management later down the line

## Features to add
- Automatic member retrieval
- Automatic filling in of the home team name

# Pages

## Landing page (Regular)
![Landing Page](/Layout/FirstPanel.png)

### Rules
- Wedstrijdnummer has to be filled in manually
- Afdeling is chosen manually from a pre-defined list
- Thuisploeg has to be picked automatically based on the user settings -> can be changed manually if needed
- Letter has to be manually picked form a pre-defined list of letters
- Bezoekers has to be manually picked from an existing list of clubs
- Players need to be filled in manually based on a list of members of the team
- Klassement, waarde, lid have to be filled in automatically based on the players chosen
- Captain has to be filled in manually from a list of the chosen players

#### Buttons
- **Bekerwedstrijd:** changes the rules to be those of a cupmatch
- **Masters:** changes the rules to be those of a masters tournament
- **Add new player to the list** -> should become obsolete with automatic retrieval of members.  Possibly keep it for when there is a lack of internet connection.
- **Afdrukken wedstrijdblaadjes:** Print the game letters with the correct info and opens the score view **SHOULD ONLY WORK IF ALL INFORMATION IS FILLED IN**
- **Ga naar wedstrijdblad:** Go to the score view without printing game letters **SHOULD ONLY WORK IF ALL INFORMATION IS FILLED IN**

## Landing page (Cup Match)
![Landing Page Cup](/Layout/FirstPanelCup.PNG)
  
### Changes
- Afdeling dissappears. Can't be filled in anymore
- Geef ronde in: New dropdown bar, you have to choose from a pre-defined list

## Landing page (Masters Match)
![Landing Page Masters](/Layout/FirstPanelMasters.PNG)

### Changes
- Afdeling dissappears. Can't be filled in anymore
- Only allowed to choose 2 players instead of 3

## Scoring page (Regular)
![Scoring page](/Layout/ScorePanel.PNG)

### Rules
- Team, Player, Rank, Value and Teamvalue have to be transfered from the landing page
- The order of games is pre-determined
- The double can be chosen manually with any of the following configurations for both teams: **1-2, 1-3, 2-3**
- Sets visually update according to the scoring
- Match updates according to the scoring. X in the right spot for the winning player, a count at the bottom.

#### Buttons
- **Terug naar ingave, alles word gewist:** Go back to the landing page, delete all inputs in the score page
- **Terug naar ingave, uitslagen worden niet gewist:** Go back to the landing page, all scores are kept in memory
- **Ingave controleren en wedstrijdblad afprinten:** Checks all scores/matches for any fault. Gives an error message and highlights the mistakes if there are mistakes. Otherwise, print the game paper.

## Scoring page (Cup Match)
![Scoring page Cup](/Layout/ScorePanelCup.PNG)

### Changes
- **Voorgift:** automatically calculate advantage based on difference in player's values
- **Ingave controleren:** checks for mistakes according to the rules of a cup match

## Scoring page (Masters Match)
![Scoring page Masters](/Layout/ScorePanelMasters.PNG)

### Changes
- **Voorgift:** automatically calculate advantage based on difference in player's values
- **Ingave controleren:** checks for mistakes according to the rules of a cup match
- Double is pre-defined as there are only 2 players/team

# Before printing the game paper

## Ending hour of the game
![End hour](/Layout/HourEnd.PNG)

### Rules
- Has to be manually given in the format XXuYY where XX = hours and YY = minutes

## Eventual accidents
![Accidents](/Layout/Accidents.PNG)

### Rules
- Prompt Yes or no for eventual accidents/comments
- If user clicks yes, show a new dialog box where they can input the comments/accidents
- If user clicks no, print the game paper
