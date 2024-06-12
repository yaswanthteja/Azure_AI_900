What follows are some high-level topics and takeaways from major areas of the exam. This should give you a picture of what’s on the exam as well as many of the AI capabilities Microsoft Azure currently offers.

### Responsible AI
One of the things I was most pleased was included on the exam was Microsoft’s principles of Responsible AI. These are a set of 6 principles that Microsoft identified governing the use of artificial intelligence technologies in applications:

- Fairness – AI should treat all groups of people fairly and not discriminate on people based on gender, ethnicity, or other factors.
- Reliability and Safety – AI should work reliably, even under extreme cases and with extreme sets of data.
- Privacy and Security – AI data sources containing personal data should be treated with respect and kept private.
- Inclusiveness – AI should be for the benefit of all people, including those with disabilities or from minorities. Solutions should be designed with these people in mind first and foremost.
- Transparency – It should be possible to determine how AI solutions arrive at the conclusions they do. Users should understand the high-level limitations of the AI systems they interact with.
- Accountability – Designers of AI solutions should be accountable for those solutions. AI solutions must work within the framework of local governments.

I personally find these principles of responsible AI very refreshing and important. In particular, recognizing the potential for bias to enter an AI system is critical when designing and testing those systems.


### Machine Learning Concepts
The exam covers the following machine learning scenarios:

- Regression – Predicting a numerical value (or label) such as a price or temperature given a set of parameters (or features).
- Classification – Evaluating a set of features to determine what class of thing a set of parameters likely belongs to. For example, given a set of parameters for a movie, determine if it is a Christmas movie or a different type of movie (stay tuned for future articles about this one).
- Clustering – Grouping together different sets of data by their similarity. For example, identifying different segments of users for marketing communications.
- Anomaly Detection – Detecting irregular data points, such as fraudulent transactions.
- Time Series Predictions – Predicting values based on historical trends.
These machine learning techniques are grouped into supervised, unsupervised, and reinforcement learning techniques. The primary difference between these techniques is that supervised learning techniques requires data to be pre-labelled for the thing you are trying to train the model to predict whereas unsupervised learning does not require this. Reinforcement learning allows machines to teach themselves by relying on some external scoring function.

Most machine learning techniques are supervised learning, but clustering relies on unsupervised learning.

The exam also covers a wide variety of metrics related to measuring the effectiveness of the various types of machine learning tasks.

### Azure Machine Learning
Azure offers a variety of things on machine learning through Azure Machine Learning Studio depending on your needs and experience level with machine learning.

![image](https://github.com/yaswanthteja/Azure_AI_900/assets/93423367/97a91b8a-e741-4d52-8c6f-1b619b17fc5f)


#### ML Studio

For experienced data scientists, Azure offers hosted Jupyter Notebooks in the Azure space where individuals can run custom Python code in an Azure environment.
![image](https://github.com/yaswanthteja/Azure_AI_900/assets/93423367/a03fd74b-dadc-44b2-8f68-b34bf230cd9e)

### Jupyter Notebook on Azure

Azure also offers a drag-and drop designer allowing data scientists to create training and evaluation pipelines that can take in data sets and perform training and predictions. This relies on some knowledge of machine learning algorithms, but does not necessarily involve coding (though Python and R programming tasks can be incorporated).
https://res.cloudinary.com/practicaldev/image/fetch/s--T2dN7Y3h--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_800/https://i1.wp.com/killalldefects.com/wp-content/uploads/2021/11/MLDesigner.png%3Fresize%3D770%252C459%26ssl%3D1
### ML Designer

For those without extensive knowledge of machine learning algorithms or those who are not certain which algorithm might be best for their needs, there is the option of Automated ML. With Automated ML Azure will automatically try different machine learning techniques until it finds one that performs well enough to meet your needs. This dramatically increases the accessibility of machine learning, though care must still be taken creating sets of data and devising machine learning experiments.

### Automated ML Configuration Screen

Azure Machine Learning Studio also offers compute and data set management as well as endpoint management for deployed machine learning solutions.

### Conversational AI
Another branch of artificial intelligence covered on the exam is that of Conversational AI. Conversational AI involves the design of chat bots that can interact with humans through various channels such as web pages, Slack, or Microsoft Teams.
![image](https://github.com/yaswanthteja/Azure_AI_900/assets/93423367/eb6ca55b-e2ee-47c6-bd16-a4606db8c448)

The conversational AI offerings are more limited, but include the Azure Bot Framework SDK, Azure Bot Service, and Azure QnA Maker. Bot framework allows you to program bots that will run on the Azure Bot Service. Azure QnA Maker can be used to generate simple bots that give answers from pre-existing word documents, PDFs, and web pages. You can also augment bots with "chitchat" profiles to allow them to respond to common queries and boost the illusion of being an intelligent agent.

### Chatbot Transcript
A sample chat application
Note that unlike most other Azure AI offerings bots do not directly integrate with Azure Cognitive Services.
![image](https://github.com/yaswanthteja/Azure_AI_900/assets/93423367/1879fa39-3a2b-4169-bf28-a2a3f92fccd7)


### Computer Vision
The exam covers computer vision fairly extensively, though it is not as much of a priority as machine learning or general AI principles. This was actually a relief since this area felt the most Azure-specific and is personally not as interesting of an area of AI compared to others despite advances every day in autonomous vehicles and similar fields. On Azure computer vision can be split into the following key areas:

- Computer Vision – pre-trained solutions that can meet a variety of needs around object detection and image classification. This can also identify celebrities and landmarks.
- Custom Vision – an area that allows you to use the capabilities of Computer Vision, but you must provide your own training images and train a vision model
- Face – specializing in face detection and analysis. This can be used to identify individuals, map landmarks of faces, identify emotions, detect glasses and makeup, classify gender, and identify similar individuals. The last two aspects of this API concerns me for obvious potential abuses, however.
- Optical Character Recognition – Allows computer vision to identify text either with its quick OCR library or the more asynchronous Read API designed to handle larger volumes of content
- Form Recognizer – a specialized area of computer vision designed to read tabular data and receipts
Overall, these are surprisingly capable solutions that can be added fairly easily to applications. I’ve just never had explicit interest in building something that requires these technologies yet.

### Natural Language Processing
Natural Language Processing (NLP) involves the understanding and translation of human text and speech. For whatever reason the inclusion of speech in this area was difficult for my mind to grasp while studying.

The most interesting parts of NLP for me revolve around the Text Analytics and Language Understanding services, but speech recognition, speech synthesis, and language translation are all part of NLP as well.

Text Analytics allows you to take some human text and detect what language it was in, identify some form of positive or negative sentiment based on the content of the text with sentiment analysis, use key phrase extraction to identify the core talking points, and use entity recognition to extract locations, people, quantities, and dates / times from text.

Language Understanding , or LUIS , allows you to take a command (also referred to as an utterance) and match it to an intent the system knows about, then extract any entities related to that intent. This allows you to take something the system may not have seen explicitly and match it to the closest registered intent, then hand off any related entities to that intent to be able to respond to the person’s text. This type of approach is at the core of things like Cortana, Alexa, and similar digital assistants.

Speech recognition , speech synthesis , and language translation are capable parts of the platform as well, with an interesting and growing array of options available to them.

### Preparing for the Exam
The AI Fundamentals certification is not currently a pre-requisite for any other certification, though it will help you get a broad overview of the AI landscape – particularly on the Azure platform. The AI-900 exam required by this certification is a relatively easy one and will also help prepare you for more specific certifications such as the Azure AI Engineer certification or Azure Data Scientist certification.

I personally took this exam to help me point any student or graduate in the direction of things that might interest them and to ensure I had a broad understanding of AI prior to starting my master’s of science in data analytics program in the new year.

If you’d like to take this exam, your first stop should be the free Microsoft Learn content listed at the bottom of the exam page. These learning paths will guide you through all of the areas of the exam, give you some practice with these tools and techniques, and present you with some quiz questions that may be similar to those on the exam.
