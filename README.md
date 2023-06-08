# Bob, the BuilderBot
## 👷🏼‍♂️ LLM-Agent for autonomous Software Creation 🏗️

Bob the BuilderBot explores how we can use LLMs to create good software. It is still in very early development.
The goal is to create an agent that takes input from an average non-technical user and creates working software for the user.

Reasonable asks from Bob the BuilderBot could be:
- "Give me a Tetris game I can play in the browser"
- "I want a website where I can track my weight"
- "For our neighborhood, we're building an item library, where you can borrow items instead of books. Can you give me a website where people can borrow items?"

The goal is **not** to build highly complex, performant or security-critical systems.
Bob will never build software to control nuclear power plants or hospitals.

## Approach

I think an agile development process works best, as:
1. Bob builds non-critical systems, and
2. the user is non-technical and therefore doesn't exactly know what they want.

To make use of Bob's services as effortless as possible, Bob should try to make educated assumptions instead of asking the user for every detail. Only when really necessary, should Bob ask clarifying questions.

With this in mind, the phases of Software Creation for Bob are:
1. **Understand:** Translate user input into a detailed requirements list & ask clarifying questions
2. **Architect:** Decide on high-level architecture and tech stack
3. **Structure Code:** Decide which files we'll need, what they'll do and what the main functions are
4. **Structure Tests:** Decide how we'll test and what tests we'll have
5. **Flesh out code:** Iteratively, write the code
6. **Flesh out tests:** Iteratively, write the tests and make sure they pass
7. **Deploy:** Deploy so user can see and interact with the project
8. **Improve:** Ask user for feedback, rinse and repeat

Theses phases only roughly correspond do traditional Software Engingeering phases, as I think that in the context of Sofware Creation via LLMs, it makes more sense to divide the process along LLM capabilites. I.e., each phase should be one action an LLM can do.

Each step is an LLM-call wrapped in [Reflexion](https://arxiv.org/abs/2303.11366).

## Problems to solve
This is an incomplete list of what's to do:

1. Finish v0
- Finish implementing all 8 phases (currently 1-3 work)
- Decide how to deploy (Streamlit? replit? ...?)

2. Improve without gradient based techniques
- Use few-shot prompting (currently zero-shot)
- Use better method for LLM inference (e.g. [Tree of Thought](https://arxiv.org/abs/2305.10601))

3. Improve with gradient based techniques
- Finetune?

4. General
- Add prioritization to requirements list (?)
- How are iterations 2+ different for the initial iteration


## How to use
todo


## How to contribute
todo


## Citation
todo

---
Twitter: [@UmerHAdil](https://twitter.com/UmerHAdil) - Feel free to reach out!
