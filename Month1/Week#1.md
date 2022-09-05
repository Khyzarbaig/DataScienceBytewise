

# What is Data Science? 
## Need for data Science

As we look around data is everywhere, its need is increased in the past 15 years due to automation and smart systems.
For example: if we talk about autonomous car, they all work on data to take decisions like speeding up and turning when it is needed and it is researched and said that autonomous cars are safer than human driven cars. Data is all it requires to train cars, models and according to which they take decisions.
For Example, when we talk about airlines, data science comes again. Flight schedule depending on weather conditions and flight route planning, it all depends on correct data output and on the bases which decision is taken 
So, to avoid most of the problems we can efficiently use data science and can make important decisions. 
They say Data is the new Oil.



## Data Science is used for
1.	Better Decision Making
2.	Predictive Analysis
3.	Pattern Discovery

A real-life example, Lets say we want to buy some furniture, we will first start to check good place or a well known website brand to buy from, we will look for rating, reviews and prices. It all comes in data, on the bases of this data we are making our decision to buy furniture from a good place in our budget.
Data science can help us find best route on a busy day or any movie recommendation and many other things.

## Important steps in Data science
1.	Asking the right question, exploring the data.
2.	Modeling the data using different techniques and algos.
3.	Finally Communicating, reporting, and visually presenting the data results.

## Business Intelligence VS Data Science 
BI was first step when people and companies started to make decisions on data and tried marketing and different techniques to get profit.

## Data sources 
* The data source for BI was Structured Data (Data Warehouse) but for Data science it was Unstructured (web, images, logos etc.).
* Method for both were different too. For BI it was Analytical(Historical data presenting the truth) but for Data science it was Scientific( Finding behaviors, insights, statistical analysis.)

## Skills
BI was all about dashboards and visualizations to present results.
Whereas in data science, there was a lot of ML, statistical analysis etc.
So, for data science skills are required more.

## Focus
* BI: Past and present data 
* Data science: Past, present and future prediction.

## Prerequisites
1.	Curiosity (To ask)
2.	Common Sense (be creative, active)
3.	Communication Skills (Asking, presenting, reporting)

## Skills Prerequisites
1.	Machine Learning 
2.	Modeling
3.	Statistics
4.	Programming 
5.	Data bases

## Data Analysis
* Skills: Python, R
* Tools: SAS, Jupyter, Excel, Python.

## Data Warehouse
* Skills: ETL, SQL, Hadoop, Apache Spark.
* Tools: Informatica/Talend, AWS Redshift

## Data Visualization
* Skills: R, Python Libraries
* Tool: Jupyter, Tableau, Cognos, RAW.
 
## Machine Learning
* Skills: Algebra, ML, Algorithms, Statistics
* Tools: Spark MLib, Mahout, Azure ML studios.


## What does a Data scientist do?
In a real world a data scientist will get a problem he needs to solve, he will understand the problem by asking questions, then he will gather the data required for the problem (Raw Data). After getting all the data from different sources he then will process and analyze the data in the form in which it is used so that its ready for going into analytical system whether it is machine learning algo or any statistical model to perform the work which will give us required results so, then the data will be meaningful. After all this its time to present and communicate the results to the stake holders, will visualize the data make useful insights.

## Important ML Algos
1.	Regression
2.	Clustering
3.	Decision Tree
4.	Support Vector Machine
5.	Naive Baiyes 


## Life Cycle of Data Science
1.	Concept study (Understand the problem properly)
2.	Data preparation (Getting data, gathering data, making data meaningful)
    * Data Integration
    * Data Transformation
    * Data Reduction
    * Data Cleaning
3.	Model Planning (EDA)
4.	Model Building
5.	 Communicating Results
6.	Operationalize 



# Probability for Data Science
## Definition:
It is the measure of the likelihood of an event.
E.g,Tossing a coin {Head, Tail}
So, 
Probability = No of ways an event can occur / no of possible outcomes
Probability = 1/2 (for head)

## 1.	Mutual Exclusive Event
Tossing a coin, so in this either Head or Tail will come no two things at a same time so it is known as mutually exclusive event.
Additive Rule
P= P of Head + P of Tail
P= ½ + ½ = 1
## 2.	Not Mutual Exclusive Event 
	Taking out a card from deck, so two cards can come at a same time.
Additive Rule 
e.g, Taking out a card from a deck
	Pr (K or Heart)
	So first find,
	Pr (K) = 4/52
	Pr (Heart) =13/52
NOW, Pr (K or Heart) = 1/52
	Pr (K or Heart) = Pr (K) + Pr (Heart) - Pr (K or Heart)
	Pr (K or Heart) = 4/52 + 13/52 – 1/52
	Pr (K or Heart) = 14/52

### Additive Rule
#### ME   Pr(A or B) = Pr(A) + Pr(B)
#### NME Pr (A or B) = Pr(A) +Pr(B) – Pr(A and B)

### Multiplicative Rule
#### 1.	Independent Event
In every calculation the probability won’t change or reduce. Its independent.
Pr(A and B) = Pr(A) x Pr(B)
#### 2.	Dependent Event 
In every calculation the probability is dependent on the last event happened, as the no of total outcomes will reduce.
Pr(A and B) = Pr(A) x Pr(B/A)

# Combinatorics
Combinatorics is mainly about counting. It deals with the arrangements of objects according to some pattern and counting the number of ways it can be done.
Enumerative combinatorics, 
## 2 Principles:
#### Addition
If a work can be done in n ways and another work can be done in m ways then either of the two ways work can be done in m+n ways.
	E1 and E2(Mutually Exclusive)
	E= E1 or E2 	
	N(E) = E1 +E2
  
#### Multiplication
If a work can be done in n ways, and another work can be done in m 
	ways, then both the operation can be done performed in nxm ways.
	Work 1 = n ways
	Work 2= m ways
	Both work1 and work2 = nxm ways.



# Python
Python is a high-level, interpreted, interactive and object-oriented scripting language. Python is designed to be highly readable. It uses English keywords frequently where as other languages use punctuation, and it has fewer syntactical constructions than other languages.

## Hello World
print("Khyzar Baig here!"). The simplest directive in Python is the "print" directive - it simply prints out a line. Print is statement not a function.
Python uses indentation for blocks, instead of curly braces. Both tabs and spaces are supported, but the standard indentation requires standard Python code to use four spaces
x = 1
if x == 1:
    # indented four spaces
    print("x is 1.")

## Variables and Types
Python supports two types of numbers - integers(whole numbers) and floating point numbers(decimals). 
myint = 7
print(myint)
myfloat = 7.0
print(myfloat)

## Strings are defined either with a single quote or a double quote.
mystring = 'hello'
print(mystring)
The difference between the two is that using double quotes makes it easy to include apostrophes (whereas these would terminate the string if using single quotes)

## List mutable Python object which can contain any type of variable and can also be iterated over. Some list methods are:
### • append(): adds an element at the end of the list
### • sort(): sorts the list in ascending or descending order
### • copy(): returns a copy of the list
### • count(): returns the number of elements with the specified value
### • pop(): removes the element from the specified position
### • reverse(): reverses the order of the list
### • index(): returns the index of the first occurrence of the specified argument 
### • insert(): adds an element at the specified position
