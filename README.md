# Tabletennis-Score-App
A rewrite of the original Table Tennis score appllication in C# with added features


# Purpose of this App
The original purpose of the app was a way to easily print match sheets for our club.
The app I'm developing will be converting visual basic to C# for easier management later down the line

## Features to add
- Automatic member retrieval
- Automatic filling in of the home team name

# Pages

## Landing page
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
- Bekerwedstrijd: changes the rules to be those of a cupmatch
- Masters: changes the rules to be those of a masters tournament
- Add new player to the list -> should become obsolete with automatic retrieval of members.  Possibly keep it for when there is a lack of internet connection.
- Afdrukken wedstrijdblaadjes: Print the game letters with the correct info and opens the score view **SHOULD ONLY WORK IF ALL INFORMATION IS FILLED IN**
- Ga naar wedstrijdblad: Go to the score view without printing game letters **SHOULD ONLY WORK IF ALL INFORMATION IS FILLED IN**
