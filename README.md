# Turning Machine Learning Models into APIs in Python
# Learn to how to create a simple API from a machine learning model in Python using Flask.
Consider the following situation:

You have built a super cool machine learning model that can predict if a particular transaction is fraudulent or not. Now, a friend of yours is developing an android application for general banking activities and wants to integrate your machine learning model in their application for its super objective.

But your friend found out that, you have coded your model in Python while your friend is building his application in Java. So? Won't it be possible to integrate your machine learning model into your friend's application?

Fortunately enough, you have the power of APIs. And the above situation is one of the many where the need of turning your machine learning models into APIs is extremely important. Many of the industries are now looking for Data Scientists who can do this. Now, wrapping a machine learning model into an API is not very difficult, and that is precisely what you will be doing in this tutorial - Turn your machine learning model into an API.

Specifically, you will be covering the following:

Options to implement machine learning models
What are APIs?
Flask basics
Creating a machine learning model
Saving the machine learning model: Serialization & Deserialization
Creating an API from a machine learning model using Flask
Testing your API in Postman
Options to implement Machine Learning models
Most of the times, the real use of your machine learning model lies at the heart of an intelligent product – that may be a small component of a recommender system or an intelligent chat-bot. These are the times when the barriers seem very difficult to overcome.

For example, the majority of the ML practitioners use R/Python for their experiments. But consumers of those ML models would be software engineers who use a completely different technology stack. There are two ways via which this problem can be solved:

Rewriting the whole code in the language that the software engineering folks work. The above seems like a good idea, but the time & energy required to get those intricate models replicated would be utterly waste. Majority of languages like JavaScript, do not have great libraries to perform ML. One would be wise to stay away from it.
API-first approach – Web APIs have made it easy for cross-language applications to work well. If a frontend developer needs to use your ML Model to create an ML powered web application, they would just need to get the URL Endpoint from where the API is being served.
Now, before going any further let's study what really is an API.

What are APIs?
"In simple words, an API is a (hypothetical) contract between 2 softwares saying if the user software provides input in a pre-defined format, the later with extend its functionality and provide the outcome to the user software." - Analytics Vidhya

You can read the following articles to understand why APIs are a popular choice among developers:

History of APIs
Introduction to APIs
Essentially, APIs are very much like web applications, but instead of giving you a nicely styled HTML page, APIs tend to return data in a standard data-exchange format such as JSON, XML, etc. Once you a developer has the desired output they can style it whatever the way they want. There are many popular ML APIs as well for example - IBM Watson's ML API which is capable of the following:

Machine Translation - Helps translate text in different language pairs.
Message Resonance – To find out the popularity of a phrase or word with a predetermined audience.
Question and Answers - This service provides direct answers to the queries that are triggered by primary document sources.
User Modelling – To make predictions about social characteristics of someone from a given text.
Google Vision API is also an excellent example which provides dedicated services for Computer Vision tasks. Click here to get an idea of what can be done using Google Vision API.

Basically what happens is a majority of the cloud providers, and smaller machine learning focused companies provide ready-to-use APIs. They cater to the needs of developers/businesses that do not have expertise in ML, who want to implement ML in their processes or product suites.

Popular examples of machine learning APIs suited explicitly for web development stuff are DialogFlow, Microsoft's Cognitive Toolkit, TensorFlow.js, etc.

Now that you have a fair idea of what APIs are, let's see how you can wrap a machine learning model (developed in Python) into an API in Python.

Flask - A web services' framework in Python:
Now, you might think what is a web service? Web service is a form of API only that assumes that an API is hosted over a server and can be consumed. Web API, Web Service - these terms are generally used interchangeably.

Coming to Flask, it is a web service development framework in Python. It is not the only one in Python, there couple others as well such as Django, Falcon, Hug, etc. But you will use Flask for this tutorial. For learning about Flask, you can refer to these tutorials.

If you downloaded the Anaconda distribution, you already have Flask installed. Otherwise, you will have to install it yourself with:
