# Overview

Authors write articles on tech topics on Devopedia. Often developers are interested in knowing how popular is that topic or how it's popularity has been growing. The goal of this project is to find this information from various sources and then plot graphs to show this.

For example, let's say we're looking at an article titled "Data Science". The algorithm would identify trends and popularity for this topic and closely related topics. Related topics could be complementary topics such as "Machine Learning" or "TensorFlow"; or could be competitive topics such as "Business Analytics" or "Data Engineering".

The algorithm must consider the following sources:
* Google Trends: show trend for the last 1 year
* GitHub/GitLab/BitBucket: projects, stars, forks, etc.
* StackOverflow: popularity based on questions, answers, votes, etc.

Use APIs instead of web scraping. When integrated into Devopedia, this code will update the trends for a topic only about once in two weeks. Hence, we need not worry about API rate limiting at this point.


# Deliverables

Project must be implemented in Python3 or Node.js with a modular design. Provide basic documentation and example graphs. 

Code should support the following:
* A module to obtain related topics.
* A module to get Google Trends for the topic and related topics.
* A module to get GitHub/GitLab/BitBucket projects.
* A module to get StackOverflow popularity.
* In all of the above, implement some form of ranking so that we can see clearly the top three items in each category.
* Save data is a suitable format.
* Plot suitable graphs in D3.js with basic hover interactions. Each graph should include date of last update.
