Most code is copied from 
https://github.com/openai/openai-realtime-console

I only corrected a following part:

1. Add text input part by adding the text input front using 
`handleTextSubmit` and `form`

2. Build Pinecone DB. Check `build-pinecone.py` file and also check the Pinecone website using our `dev_team@circle.net` account using google login.

3. Add `flask_app.py` to run the flask server to query to Pincone Vector DB when it's requested by the agent (realtime api)

To run, follow the steps below:

1. Create `.env` file with OPENAI_API_KEY and PINECONE_API_KEY

2. Run `npm install`

3. Run flask app `python flask_app.py`

3. Run `npm start` 

Then the app will run on `localhost:3000`
