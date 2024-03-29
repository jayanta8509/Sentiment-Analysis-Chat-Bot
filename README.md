Install Dependies : 
langchain
langchain-google-genai
streamlit
python-dotenv
huggingface_hub

Model used for text generation - "gemini-pro"
Model used for sentimental analysis - "lxyuan/distilbert-base-multilingual-cased-sentiments-student"

I have not used any prompt because "gemini-pro" does not support prompt template and for sentimental analysis i have used "lxyuan/distilbert-base-multilingual-cased-sentiments-student" this model from hugging face.



# Code Explanation:
# At first i have import necessary libraries, and "hugging face" API and "gemini-pro" API
# To build the chatbot i have used LangChain 
# Using LangChain I hit the "gemini-pro" model for text-to-text generation
# After I got the result , stored it in a variable. 
# This variable is further used for sentimental analysis of the generated text 
# For sentimental analyis first i have initialized the model through my hugging face API. After the initialization i have hit the sentimental analysis model with the variable(generated text of chatbot) which gives "Positive Value" ,"Negative Value" and "Neutral Value" of that text.
# Positive Value denotes positive sentiments of a text , Negative Value denotes negative sentiments of a text , Neutral value denotes neither positve nor negative sentiments related to that text.
# At last I have used streamlit to display the visual representation of the overal model.
link : https://sentimentachatbort.streamlit.app/




