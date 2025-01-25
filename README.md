[![CodeFactor](https://www.codefactor.io/repository/github/ggeop/python-ai-assistant/badge)](https://www.codefactor.io/repository/github/ggeop/Python-ai-assistant)
[![Maintainability](https://api.codeclimate.com/v1/badges/8c90305e22186cc2c9d5/maintainability)](https://codeclimate.com/github/ggeop/Python-ai-assistant/maintainability)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://app.travis-ci.com/ggeop/Python-ai-assistant.svg?branch=master)](https://app.travis-ci.com/ggeop/Python-ai-assistant)

![alt text](https://github.com/ggeop/Python-ai-assistant/blob/master/imgs/jarvis_logo.png)

# About Jarvis - An Intelligent AI Consciousness 🧠
Jarvis is a voice commanding assistant service in [Python 3.8](https://www.python.org/downloads/release/python-360/)
It can recognize human speech, talk to user and execute basic commands.

#### Requirements

* Operation system: **Ubuntu 20.04 (Focal Fossa)**
  


#### Assistant Skills 
*   **Opens a web page** (e.g 'Jarvis open youtube')
*   **Tells about something**, by searching on the internet (e.g 'Jarvis tells me about oranges')
*   **Tells the daily news** (e.g 'Jarvis tell me today news')
*   **Spells a word** (e.g 'Jarvis spell me the word animal')
*   **Creates a reminder** (e.g 'Jarvis create a 10 minutes reminder')
*   **Opens linux applications** (e.g 'Jarvis open bash/firefox')
*   **Tells everything it can do** (e.g 'Jarvis tell me your skills or tell me what can you do')
*   **Tells the current location** (e.g 'Jarvis tell me your current location')


#### Assistant Features
*   **Asynchronous command execution & speech recognition and interpretation**
*   Supports **two different user input modes (text or speech)**, user can write or speek in the mic.
*   **Keeps commands history and learned skills** in MongoDB.'

## Getting Started
### Create KEYs for third party APIs
Jarvis assistant uses third party APIs for speech recognition,web information search, weather forecasting etc.
All the following APIs have free no-commercial API calls. Subscribe to the following APIs in order to take FREE access KEYs.
*   [OpenWeatherMap](https://openweathermap.org/appid): API for weather forecast.
*   [WolframAlpha](https://developer.wolframalpha.com/portal/myapps/): API for answer questions.
*   [IPSTACK](https://ipstack.com/signup/free): API for current location.



### Start voice commanding assistant
![alt text](https://github.com/ggeop/Jarvis/blob/master/imgs/Jarvis_printscreen.PNG)

*   Start the assistant service:
```bash
bash run_jarvis.sh
```



### Decision Model
![alt text](https://github.com/ggeop/Jarvis/blob/master/imgs/desicion_model.png)

### Extract skill
The skill extraction implement in a matrix of [TF-IDF features](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) for each skill.
In the following example he have a dimensional space with three skills.
The user input analyzed in this space and by using a similarity metric (e.g cosine) we find the most similar skill.
![alt text](https://github.com/ggeop/Jarvis/blob/master/imgs/skill_space_desicion.png)



</div>

