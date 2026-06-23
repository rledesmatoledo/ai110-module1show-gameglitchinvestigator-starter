# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

  - When I first ran the game I kept the mode on normal and the secret number was 65. I guessed 60 and were told to guess lower instead of higher and vice versa when i guessed 66. I also noticed that when the difficulty level is changed the guesses are still being asked in the 1-100 normal mode format. When starting a new game it doesnt reset history and sometimes does not even let me guess.

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|guess of 60(secret number = 65)|Go higher hint given|Go lower hint|no errors|
| Change difficulty to Easy or Hard|Guess range should change to match the selected difficulty| Program still prompts to guess in the normal 1–100 range|No errors |
| Start a new game|Previous guesses are cleared & game should accept new guesses|Guess history from previous game is stil there & sometimes does not allow new guesses|No errors but is unresponsive at times |
|Guess of 66(secret number = 65)|Go Lower | Go higher| no error|

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
I decided to use Claude built into vs code which is more flexible. All the AI suggestions were pretty much correct, I believe this is because the code isnt long and opening the new tabs helped keep the memory intact for each task. The way that I could tell was by me just reading the fix and the logic and it made sense. For example, the error of the too high or too low logic was fixed quick with AI because its logic was reversed.

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?
The way I could tell was reading the reasoning behind the fix and also checking out if any changes were actually made. Used the pytest errors and plugged into AI to get an explanation and possible help with the error. AI definetly helped me understand what was actualy wrong.
---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
Streamlit reruns the script whenever a click is made to the app itself.
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
A stratedgy from this project that I want to reuse in future labs or projects is to use new tabs in claude to tackle different problems. Making it focus on one bug at a time to avoid any hallucination and crossing the bug fixes or error. My view on AI code has changed a bit because I have a better version of the AI mode so code is better but I still am going to be catious of certain errors and hallucinations.