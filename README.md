# Udacity Data Analyst Nanodegree DANDP8
## Anna Lisboa Signor

## Bubble Chart of Customer Support Cases, Dynamic Filter on Satisfaction


As a data analyst in a service and data-driven environment, I often receive requests for visualizations of "the customer's experience with cases". In fact, customer support data is one of the most in-demand types of data corpuses from which to derive information in my line of work. Although the operation generating the data may not seem complex, the way the data may translate into insight is far from straight-forward.

Managers, executives, and agents on the field sense a customer's dissatisfaction and the need arises to understand why. What often happens following this is a request to see a lot more information than what can fit in a chart that makes sense: how many cases, how long they were open, how long it took to respond, are they satisfied, level of dificulty and effort. The problem is all these quantitities and attributes are not independent from one another, and many of them do not have an operation definition with which the entire audience is in accordance. To make matters more complicated, a case spans a period of time, rather then be associated with one date or time. This makes the question "how many cases this month?" a lot more complex than it looks at face value.

In this sample visualization, I showcase one of the charts I have developed in answer to the challenge above. The goal for this visualization is to show a measure of how many cases are open in a time period and how long they were open, both. So there is insight into how many issues a customer is experiencing, as well as how long they had to wait for a resolution. A third piece of information is introduced in the form of a dynamic series, which is interactive: the data consumer can toggle three different satisfaction categories in and out of the chart.

To see the visualization, serve up DANDP8.html to a browser and have customer_support.csv in the same folder. All the styling and scripts are in the html file.

Customer_support.csv is sample customer support data and the organization will remain anonymous.

References:
http://dimplejs.org/
https://stackoverflow.com/questions/30090642/customizing-colors-on-dimple-js-charts/30103957#30103957
