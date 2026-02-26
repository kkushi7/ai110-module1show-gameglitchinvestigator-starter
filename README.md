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
- [ ] Detail which bugs you found.
- [ ] Explain what fixes you applied.

## 📸 Demo

- [ ] [Insert a screenshot of your fixed, winning game here]

## 🚀 Stretch Features

- [ ] [If you choose to complete Challenge 4, insert a screenshot of your Enhanced Game UI here]


Phase 1:
Four bugs that I found were that the attempts count did not change after giving the first attempt causing it to miscount, the new game button does not restart the game properly once over with a round, as it still says game over and to restart the game, the hints are not proper as it says to go higher when we should be going lower and vice versa, and the enter button does not work to enter your guess, as you have to manually click the submit guess button.


Phase 2:
Some guiding hints I would give to students would be to look over the functions within app.py to help them spot the area or function in which would make sense for them to look over to fix their bugs. This also will help them when prompting AI, as it will be more clear for both parties as they give specifications. Another guiding hint when it comes to prompting AI would be to give it the issues and then first ask it to explain in simple terms how to fix this issue without implementation. This can help students to actually understand what the AI is doing as well as help teh AI work better with specification as it is breaking down the problem first before implementing the code right away. 
