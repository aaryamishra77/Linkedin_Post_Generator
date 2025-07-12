# Linkedin_Post_Generator
An end-to-end Gen AI project that generates professional LinkedIn posts using LLaMA 3.2, Langchain, Streamlit, and Groq Cloud. Enter a few details and get high-quality, ready-to-post content in seconds. Fast, customizable, and built with open-source tools.
This tool will analyze posts of a LinkedIn influencer and help them create the new posts based on the writing style in their old posts
<img width="1354" height="539" alt="image" src="https://github.com/user-attachments/assets/e187a449-53b6-4949-96eb-1ad209156e0a" />
Let's say Mohan is a LinkedIn influencer and he needs help in writing his future posts. He can feed his past LinkedIn posts to this tool and it will extract key topics. Then he can select the topic, length, language etc. and use Generate button to create a new post that will match his writing style.

Technical Architecture
<img width="765" height="461" alt="image" src="https://github.com/user-attachments/assets/40050524-7005-43a2-b6fa-a599d6f3e87e" />

Stage 1: Collect LinkedIn posts and extract Topic, Language, Length etc. from it.
Stage 2: Now use topic, language and length to generate a new post. Some of the past posts related to that specific topic, language and length will be used for few shot learning to guide the LLM about the writing style etc.

Set-up
To get started we first need to get an API_KEY from here: https://console.groq.com/keys. Inside .env update the value of GROQ_API_KEY with the API_KEY you created.
To get started, first install the dependencies using:

pip install -r requirements.txt

Run the streamlit app:

streamlit run main.py
