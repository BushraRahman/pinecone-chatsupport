# pinecone-chatsupport
HOW TO RUN:
In the repo, create a file called .env.
Values in .env:
PINECONE_API_KEY=  
PINECONE_INDEX_NAME=  
PINECONE_ENVIRONMENT=  
OPENAI_API_KEY=  
COHERE_API_KEY=  

Fill in those values.  
To get the Pinecone values [Instructions can also be found at https://pypi.org/project/pinecone-client/]

In the terminal, assuming you have pip, run:  
pip3 install "pinecone-client[grpc]==3.0.0.dev4"  
Sign up for a pinecone account at https://app.pinecone.io. The API Key can be found in the API keys section, you can create an index in the indexes section and PINECONE_INDEX_NAME is what you named that index, and PINECONE_ENVIRONMENT is the region (ex: us-east-1).

Cohere:  
Sign up for an account at https://dashboard.cohere.com/. The API key is in the API Keys section. 

Dependencies:  
This repo requires you to install a lot of packages, and I unfortunately did not write them all down, but here's a small list... install more packages as you run into errors.  
pip install "pinecone-client[grpc]""==3.0.0.dev4 pandas numpy pyarrow python-dotenv tenacity ray BeautifulSoup4

Order to run the files:  
First run test.py. Then run server.py: server.py will call chain.py