# Statistical-Analysis-using-GLTR-HarvardNLP

**I am testing GLTR model with text prediction on various text like journalism, TV program transcripts, and books'exerpts.**

**Giant Language model Test Room**
**Installing GLTR**

Before we can use GLTR, we need to install it on our system. Start by cloning the GitHub Repository of the project:
```
git clone https://github.com/HendrikStrobelt/detecting-fake-text.git
```

Once you have cloned the repository, cd into it and do pip install:
```
cd detecting-fake-text
pip install -r requirements.txt
```

Next, download the pre-trained language model. You can do it by running the server:
```
python server.py
```

GLTR currently supports two models – BERT and GPT-2. You can choose between the two; if no option is given then GPT-2 is used:
```
python server.py --model BERT
```

This will start downloading the respective pre-trained model on your machine. Give it some time if you have a slow internet connection.
When everything is ready, the server will start at port 5001 and you can directly go to http://localhost:5001 to access it:

Below are my trials on the transcripts on the American TV show *The Good Doctor* and on the excerpt of the book *Nudge*:

<img width="567" alt="TheGoodDoctorTranscript1" src="https://user-images.githubusercontent.com/47131675/83286019-45c25800-a1ad-11ea-8f0b-bba2d4907317.png">

<img width="491" alt="Nudge_Excerpt" src="https://user-images.githubusercontent.com/47131675/83314078-bb96e580-a1e6-11ea-8a0d-3a322f610c54.png">

As you can see that it is interestingly harder for a model to predict transcripts like human's language, but easier for it to pick up what it is in a book and predict the next words.  
