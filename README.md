# Generative-AI

## LLMs
1. Customer Care Automation :
   
   It's a voice-based solution where users can ask queries about any product specifications/order status/Return-Refund Status etc.
   - User query category identification using Langchain with OpenAI API
   - Selecting and integrating the specific database table as per the user query category
   - Used Langchain with OpenAI API to generate SQL query for the corresponding user query
   - Generated natural response using Langchain with OpenAI API

2. Ask Current Affairs :
   
   It's an LLM-based project where users can ask for current news for any categories like Sports/Entertainment/Business/Politics etc.
   - OpenAI API chat model is not trained on the latest news, It doesn't generate proper responses about current affairs.
   - Used some Python Packages to scrap daily news for different category
   - Organized the raw news texts and split them into chunks with a limited number of tokens using Tiktoken 
   - Used OpenAI Embedding model(text-embedding-ada-002) to generate embeddings of this organized news text
   - Used Cosine distance similarity score to retrieve top-n results corresponding to the query asked by the user
   - Generated response using OpenAI Chat Completion API with the above top-n results as context.

3. Ask Questions from multiple PDFs :

   It's an LLM-based project where users can upload a folder containing multiple PDFs and ask questions about the relevant topic
   - Used Langchain PyPDFLoader to load documents, split the text into smaller chunks using RecursiveCharacterTextSplitter, and create vectordb using DocArrayInMemorySearch
   - Generate the response using ConversationalRetrievalChain with custom memory handling
   - Tested by uploading a folder containing 10 Deep deep-learning papers

4. Ask Questions from Youtube Video content:

   It's an LLM-based project where users can pass multiple YouTube video URLs and ask questions about the relevant topic
   - Used Langchain YoutubeLoader to load text contents from the YouTube videos, split the text into smaller chunks using RecursiveCharacterTextSplitter, and create vectordb using DocArrayInMemorySearch
   - Generate the response using ConversationalRetrievalChain with custom memory handling
   - Tested by passing 2 YouTube video URLs for Machine Learning Tutorial
     
5. Social Media Post Writer :
   
   It's an LLM-based project that can be used to write engaging posts for different social media like LinkedIn/Twitter/Instagram.
   - User can select multiple options like Platform for which the post has to be written, in a specific tone, for the target public,
     in a limited number of words etc.
   - Generated automatic efficient and relevant prompts using Langchain
   - Used Langchain with OpenAI API to generate the relevant posts
  
6. Movie Story, Plot, Character, and Scene Generation :
   - Given a summary of a story, It generates an attractive title for the story
   - Given the story's summary and few-shot examples of the story's character with a short description, We generate a mind-blowing
     character's name and description for our story.
   - Visualize character using Stable Diffusion (Attractive Image)
   - Given the character's description and one-shot example of story breakdown into place, plot, and beats,
     We generate story beats for our story
   - Given few-shot examples of places with their description, We generate place descriptions for our story
   - Given the place description, Generated the place's scene using Stable Diffusion (Attractive Image)
   - Given a one-shot example of a scene with the corresponding dialogue among the characters, We generate
     dialogues for our scene, place, and characters.

### Concepts Learned :

1. Prompt Engineering
2. Prompt Chaining
3. Vector Database & Indexing
4. Similarity Search and LLM-based Retrieval
5. Retrieval Augmented Generation (RAG)
6. Context formation with Tabular Database, JSON Data format, and plain text
7. SQL query generation for natural language
8. Response Generation based on custom context
9. LORA, QLORA,finetuning off LLMs.


## Stable Diffusion
Tried Stable Diffusion and its variants using Huggingface Diffusers Library
- Text prompt based Image generation
- Image generation using text prompt with different controlling/conditioning factors
  like, pose, segmentation map, depth map, scribble, etc.


