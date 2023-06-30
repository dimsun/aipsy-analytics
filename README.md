# aipsy-analytics
Analytics repository

# Target:
- an interlocutor who maintains a conversation.
- concludes a contract (one of the chosen ones at the start): explore life scenarios, analysis of the situation, support. +voices the project's disclaimer: You can use this at your own risk.
- says in the voice of a psychologist (Freud? Perls? Nifont? Oprah?)
- evaluates the interlocutor according to his story
- able to ask clarifying questions
- avoids the themes of death and violence, sends to people. public psydb?
- multilingual (but how to take into account local jokes?)


# Architecture:
An analogue of chatgpt, retrained on the records of client sessions (where can I get the dataset?). A separate algorithm keeps track of the metrics. Based on the metrics, answers instead of chatgpt: "tell me more about ...", "I think ...", etc.
Prototype: listens to the speech of the interlocutor, processes, sends chatgpt for an answer with the instruction "I am a psychologist and sometimes you need to answer the client instead of me. Partially, I will answer the client myself. When I need you to answer instead of me, I will send my dialogue with the client" . Starts a temporary client profile, writing metrics there. Based on algorithms, it can answer itself using queries. When the algorithms do not issue a weighty request, the response is redirected to chatgpt listing the text of the conversation.


# Realisation:
- get a set of client session data
- get an analogue of gpt, with the possibility of additional training
- find the competence of continuing education
- find the environment deployment competency
- writing metrics tracked by aipsy

