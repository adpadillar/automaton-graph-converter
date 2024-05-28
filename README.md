# Project 3 Converter

## Team

- Axel Daniel Padilla Reyes A01642700
- Karen Corona Espinoza A01642461
- Diego Iván Morales Gallardo A01643382

## Description

This project is a web application using the `shiny` for converting some production rules into an automaton.
Then, this automaton is graphically represented using the `visual-automata` library.

### Important notes

1. This project does not use the `R` programming language, but the `shiny` library for Python. We checked with the professor and he said it was okay to use it.
2. This project reuses the `automaton.py` and `state.py` from our `Lexical Analyzer` project.
3. The only significant modifications to the `automaton.py` would be the modificaation of the `graph()` method to use the `visual-automata` library.
4. The `app.py` is the entry point for the `shiny` application. It includes the parsing of the production rules and the conversion to an automaton, as well as calling the `graph()` method to display the automaton.
5. The final state `Z` is denoted by a double circle in the automaton, instead of it being colored in red. We checked with the professor and he said it was okay to do it this way.
6. The initial state `S` is denoted by an arrow pointing to it in the automaton. We checked with the professor and he said it was okay to do it this way.

## Steps for running

1. Run these commands

```bash
git clone git@github.com:adpadillar/lexical_analyzer-py.git # clone the repo
cd lexical_analyzer-py # change to the project directory
python3 -m venv .venv # create virtual environment
source .venv/bin/activate # activate virtual environment
pip install shiny visual-automata forbiddenfruit frozendict # install dependencies
shiny run app.py
```

2. Open the browser and go to `http://localhost:8000/`
