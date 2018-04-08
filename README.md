 # Udacity Data Analyst Nanodegree DANDP8
 ## Anna Lisboa Signor
 
## About the data and the chart

The goal for this visualization is to show a measure of how many cases are open in month,how long it takes to resolve then on average, how each impacts the customer satisfaction. Since I have three features, and I need the x axis for the months, I set on a bubble chart plus a color series. 

Powering the chart is sample data from an anonymous SaaS (Software as a Service) provider, in regards to the customer support they provide. Four features appear in this visualization:

- Satisfaction: how the customer rated the service
- Month: the month when the case was opened
- Cases Count: a count of how many caases were opened in a given month 
- Time to Resolution: how long it took resolve the case, in number of hours

Here is hor they map into the chart elements:

- Satisfaction: color, dynamic filter at the legende
- Month: x axis
- Cases Count: y axis
- Time to Resolution: bubble size (radius)

 
## Finding: 
Number of cases seems to have a more immediate effect in satisfaction than the amount of time it takes to resolve.

## How to see it:
Observe how there is a clear trend of the orange bubbles centers sitting above the ones of the green and the gray bubbles. On the other hand, many of the biggest bubbles for each month are not orange. Where the visual comparison is less than obvious, you can hover your mouse and check the values. Orange actually rarely wins.

## Design iterations and process

As a data analyst in a service and data-driven environment, I often receive requests for visualizations of "the customer's experience with cases". In fact, customer support data is one of the most in-demand types of data corpuses from which to derive information in my line of work. Although the operation generating the data may not seem complex, the way the data may translate into insight is far from straight-forward.

Managers, executives, and agents on the field sense a customer's dissatisfaction and the need arises to understand why. What often happens following this is a request to see a lot more information than what can fit in a chart that makes sense: how many cases, how long they were open, how long it took to respond, are they satisfied, level of dificulty and effort. The problem is all these quantitities and attributes are not independent from one another, and many of them do not have an operation definition with which the entire audience is in accordance. To make matters more complicated, a case spans a period of time, rather then be associated with one date or time. This makes the question "how many cases this month?" a lot more complex than it looks at face value.
 
In searching for compelling and effective visualization to solve this need, I played with several complicated ideas, trying to render as much information as possible in one place, and exploring the use of animation as the represenation of time (which would free up x, y or eliminate the need to present a snapshot). This turned out to be a mistake. Specially all the time animations, although they seem "cool" they are not palatable for managers and executives, and very hard to interpret. Here is someof the feedback I received alongside sketches of defunct charts:

1. The "Efervescent Timeline" (the bottom, please ignore the top)
![](https://github.com/asignor/DANDP8/blob/master/efervescent_timeslide_and_stack_bar.jpg)

The idea for this chart was to cut up the body of cases into categories for each case type and, with one bubble per case, have it move up in the y axis according to the case age. When the case is solved, the bubble would "pop". A calendar indicator would tell the user at what point in time you are, as well let you move to a snapshot of a certain day. User would have the option to slide a bar, or let it "play" at a certain rate. I though this would give a great idea of the experience of the customer. Here is the feedback I received from different co-workers (I did not get their permission to put their name on Github):

- Person A: This is very cool, but what actual insight can I get from it? It is not metric-driven.
- Person B: I don't understand that al all. What a I looking at?

My lesson from this feedback is time animation are cool but offer no valuable insight, at least not in the ways I had thought about.

2. The "Stacked Timelines with a Siliding Aggregator"
![](https://github.com/asignor/DANDP8/blob/master/stacked_timelines_sliding_aggregator.jpg)

In this chart, the cases are represented as lines that start when a case is created and end when they are solved. So, at a glance, the consumer could see how long a case was open (length of the line). In addition, a vertical bar that can be slid side to side would aggregate information from any cases it's crossing. This way, the consumer could see metrics such as number of cases open, average age of active cases, and many more, for one slice of time. I got very similar feeback:

- Person A: There is too much information, it is confusing. I know the business is asking to see all this information in one chart, but frankly they don't always know what they want, they know what insight they need. It's your job to make that happen from approachable information

- Person B: what is on Y? I want to hink that a case that is higher up above another is there for a reason. This is a bit confusing, you need mroe straight-forward aggregation

I learned a lot from this input, the biggest lesson being the cases always need to be aggreagated. All views that try to convey anything by displaying them as indivisual elements is confusing for most people.

3. The chart in this project
I got some great feedback from the Udacity reviewer after my first publication. Main points:

	- communicate a clear finding
	- offer more information on the data (there was confusion as to what "good" and "bad" meant)
	- more details on the design and the proccess of consuming feedback to get to this state

 Upon receiving this feedback I improved this readme file to include the design process and feedback absorbed along the way, as well as an explanation of the finding.
 


 To see the visualization, serve up DANDP8.html to a browser and have customer_support.csv in the same folder. All the styling and scripts are in the html file.
 
 Customer_support.csv is sample customer support data and the organization will remain anonymous.
 
# References:

http://dimplejs.org/

https://stackoverflow.com/questions/30090642/customizing-colors-on-dimple-js-charts/30103957#30103957

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#images
 
