# Contexto_3lang
implementation of Contexto (guess the word game) for three different Languages (Arabic, English and Russian).

#### Problem description:
Contexto is word-based game in which players have to guess a secret word within an unlimited number of guesses, 
each time a player would guess a word, he will receive a number which indicates the similarity between his guess and the secret word, 
the similarity score is calculated by the back-end language model based on contextual relevance between the player guess and the final word from thousands of pre-analyzed texts.

#### The Task:
Development of a web application that represents Contexto game in three different languages, and study the optimal gaming strategies.

#### The solution:
1. derive most common words for each language to be used by the back-end model as a secret word dataset.
2. preform NLP stemming on the list of the common words for the three languages [example: Arabic](https://github.com/FaresGh1997/Contexto_3lang/blob/main/Arabic_Process.ipynb), which helps in finding the root version of the word. Pay attention, the root version of the word is heavily reliant on the language and it's grammar.
3. fine-tune a [Bert-based](https://huggingface.co/models?search=bert) model (Transformer model) for each of the three languages in order to retrieve the contextual embeddings for the words of the language.
4. use the embeddings retrieved in the previous step to calculate cosign similarity between the player word and the secret word.
5. implement the front-end part of web application by using [streamlit library](https://streamlit.io/).
6. player simulation and a study of the different [gaming stratiges](https://github.com/FaresGh1997/Contexto_3lang/tree/main/Strategies) including Maximum likelihood using (MLU) and Player Rank Using (PRU) for each of the three languages under study.

#### The final product:

Final product can be seen using [Deployment code](https://github.com/FaresGh1997/Contexto_3lang/blob/main/Deployment.ipynb), or be running the code on local machine.

![229601541-f1082ad1-8637-4bd7-9ad9-66b1b64e35f7](https://github.com/FaresGh1997/Contexto_3lang/assets/114985388/40b77736-49a6-459f-a5b8-78778ddccbd6)


Skills developed: NLP | Model Deployment | streamlit | pandas | pytorch | numpy | model-finetuning | LLM | word-embeddings | Bert-based models | Transformers | HuggingFace | genism | nltk | python.




