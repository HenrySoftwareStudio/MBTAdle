# Subwaydle

A Wordle-inspired NYC Subway daily puzzle game inspired this game: the MBTAdle. It is the same concept but for the "T" (Commuter rail doesn't count, but the Silver Line is included). Contains some source code lifted from the [open-source clone](https://github.com/cwackerfuss/word-guessing-game) by Hannah Park.

See it live at ~~https://www.subwaydle.com~~ (Website to be founded, this link goes the inspiration's site.)

## Running locally

`````
brew install yarn
yarn install
yarn start
`````

* To show the map that is displayed after finishing the puzzle: sign up for an account with [Mapbox](https://www.mapbox.com), get a token and add it to an `.env` file as `REACT_APP_MAPBOX_TOKEN`.

* Ruby scripts in the `scripts/` directory produce the JSON files in `src/data` that are used by the app. *Warning:* viewing the `src/data` can reveal spoilers to the puzzle! All guesses are checked against the keys in the respective `solutions.json` file to be a valid trip, and the `answers.json` contains an array for the answer of each day. The values of the `solutions.json` object contain an example trip of stations that are traveled through for the trip.

Permission to be secured.

Inspirations:
* [Wordle](https://www.powerlanguage.co.uk/wordle/)
* [Chengyu Wordle](https://cheeaun.github.io/chengyu-wordle/)
* [Nerdle](https://nerdlegame.com/)
* [Subwaydle](https://www.subwaydle.com)
