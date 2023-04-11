# Chatbot
To use the chatbot, you need to have [python 3.11](https://www.python.org/downloads/) installed.

First clone or download the repo to your local machine and cd into the folder.

## Environment setup
Open a terminal, use the following command to create a virtual environment and install required packages.

```bash
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```
## Run the app
Open `app.py` and update your OpenAI API key on
`openai.api_key = 'your key here'`.

Save the file and run the following code in a terminal
```bash
flask run -p 8000
```
If everything is set up correctly, you should see the following message
```bash
 * Running on http://127.0.0.1:8000
```
Then go to a web browser and nevigate to http://127.0.0.1:8000. You should be able to type in questions, press enter and get responses.
The chat history is displayed on the browser and it will be erased if you refresh the webpage.

### app.py
You can change the settings in `app.py` to fit your need.
The model used in the current file is `gpt-3.5-turbo`, `max_tokens` is set to `200` and `temperature` is set to `0.7`.


