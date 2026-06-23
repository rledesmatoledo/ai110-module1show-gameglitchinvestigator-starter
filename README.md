# 🎮 Game Glitch Investigator: The Impossible Guesser

## 🚨 The Situation

You asked an AI to build a simple "Number Guessing Game" using Streamlit.
It wrote the code, ran away, and now the game is unplayable. 

- You can't win.
- The hints lie to you.
- The secret number seems to have commitment issues.

## 🛠️ Setup

1. Install dependencies: `pip install -r requirements.txt`
2. Run the broken app: `python -m streamlit run app.py`

## 🕵️‍♂️ Your Mission

1. **Play the game.** Open the "Developer Debug Info" tab in the app to see the secret number. Try to win.
2. **Find the State Bug.** Why does the secret number change every time you click "Submit"? Ask ChatGPT: *"How do I keep a variable from resetting in Streamlit when I click a button?"*
3. **Fix the Logic.** The hints ("Higher/Lower") are wrong. Fix them.
4. **Refactor & Test.** - Move the logic into `logic_utils.py`.
   - Run `pytest` in your terminal.
   - Keep fixing until all tests pass!

## 📝 Document Your Experience

- [ ] Describe the game's purpose.
The purpose of the game is to let users guess a random generated number while receiving Lower or Higher hints.
- [ ] Detail which bugs you found.
   - The lower and higher hints were reversed.
   - The difficulty was always 1-100 no matter the mode change.
- [ ] Explain what fixes you applied.
 - Refactored check_guess into logic_utils.py.
 - Corrected the higher/lower hint logic.
 - Fixed the difficulty prompt.

## 📸 Demo Walkthrough

Describe your fixed game in numbered steps so a reader can follow along without watching a video:

1. User enters a guess of 80
2. Game returns "Go Lower"
3. User enters another guess of 70
4. Game returns Go Higher
5. Game ends after correct guess -> oututs score

**Screenshot** *(optional)*: <!-- Insert a screenshot of your fixed, winning game here -->

## 🧪 Test Results

========================================================================================= test session starts =========================================================================================
platform darwin -- Python 3.9.6, pytest-8.4.2, pluggy-1.6.0
collected 5 items                                                                                                                                                                                    
tests/test_game_logic.py .....                                                                                                                                                                  [100%]

========================================================================================== 5 passed in 0.00s ==========================================================================================

## 🚀 Stretch Features

- [ ] [If you choose to complete Challenge 4, describe the Enhanced UI changes here — a screenshot is optional]
