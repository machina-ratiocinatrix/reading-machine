# Reading-Machine
A machine that reads texts analytically and syntopically.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Are language models seeking the Truth, machine?" \
  | uvx reading-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
python3 -m pip install --user git+https://github.com/machina-ratiocinatrix/reading-machine.git
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
reading-machine multilogue.txt
```
Or:
```bash
reading-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | reading-machine
```
Or:
```bash
cat multilogue.txt | reading-machine > multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Reading-Machine?") \
  | reading-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | reading-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | reading-machine > multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | reading-machine \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import reading_machine
```
