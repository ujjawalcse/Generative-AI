# Generative-AI

## LLMs
1. Customer Care Automation
   It's a voice-based solution where users can ask queries about any product specifications/order status/Return-Refund Status etc.
   - User query category identification using Langchain with OpenAI API
   - Selecting and integrating the specific database table as per the user query category
   - Used Langchain with OpenAI API to generate SQL query for the corresponding user query
   - Generated natural response using Langchain with OpenAI API

2. Ask Current Affairs
   It's an LLM-based project where users can ask for current news for any categories like Sports/Entertainment/Business/Politics etc.
   - OpenAI API chat model is not trained on the latest news, It doesn't generate proper responses about current affairs.
   - Used some Python Packages to scrap daily news for different category
   - Organized the raw news texts and split them into chunks with a limited number of tokens using Tiktoken 
   - Used OpenAI Embedding model(text-embedding-ada-002) to generate embeddings of this organized news text
   - Used Cosine distance similarity score to retrieve top-n results corresponding to the query asked by the user
   - Generated response using OpenAI Chat Completion API with the above top-n results as context.
  
3. Social Media Post Writer
   It's an LLM-based project which can be used to write engaging posts for different social media like LinkedIn/Twitter/Instagram.
   - User can select multiple options like Platform for which the post has to be written, in a specific tone, for the target public,
     in a limited number of words etc.
   - Generated automatic efficient and relevant prompts using Langchain
   - Used Langchain with OpenAI API to generate the relevant posts
  
4. Movie Story, Plot, Character, and Scene Generation
   


