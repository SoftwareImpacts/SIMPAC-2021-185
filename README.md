# P5
An Analysis on Newly Emerged Rumors on Twitter

This is an eleven-stage project that has been devised to first make a newyly-emerged rumor dataset out of Twitter and then do a set of analysis (Micro + Macro) on it. These eleven stages (from S4 to S14), each one comes with a distinct python code with the following short decription for each one :

S4 : This code crawls the tweets related to the rumor we want to hunt. But prior to the running of the code we should have made a Twitter API so the API keys be set in the code. Also we would need to set the queries (key words related to the rumor) in the code, so to capture only those tweets that include the queries. The output which is the collection of all tweets related to the rumor will be ready in a .jsonl file.

S5 : This code by getting the S4 output as its input, seperates the data into meaningful pieces of information and then organizes them in an excell file. This excell file assigns one distinct row for each tweet and save its information (including tweet ID, User ID, Date amd Time and ...) in the columns.

S6 : This code by getting the S5 output as its input, picks up a set of tweets to then get used for human annotation. The seleccting strategies is based on the fact that tweets with more ferequencies of occures in the dataset are in priority since annotating them by human would have left less tweets for machine and the overall accuracy of the dataset would be higher. However the specified size for this pack of selected tweets and the desire to have tweets from all kinds (even those with less frequency) lead the code to choose the most appropriate tweets. This code also provides another output that is the collection of all tweets of the dataset minus the repetitive versions. This collection can be used when human anotators want to annotate whole the dataset all by their own as we would see in S6-1 (without using machine)
