Infomation Visualization Basic
==============================

coursera **[Information Visualization: Foundations](https://www.coursera.org/learn/information-visualization-fundamentals/)** course fundamental concepts by **Enrico Bertini** at New York University Tandon School of Engineering

What is Information Visualization?
----------------------------------

> "The use of computer-supported, interative, visual representations of abstract data to amplify cognition"

-	정보 시각화는 다섯 개의 주요 개념들을 통해서 설명될 수 있는데, 그 중 몇 몇 개념들의 의미는 아래와 같다.  

### Abstract Data

```
Representing visually data that does not necessarily have a very natural
or obvious visual representation.
```

-	물리적으로 보이지 않는 추상적인 데이터를 어떻게 표현할까?
-	예를 들어 시간이라면 어떻게 표현되어야 가장 적합할지 고민이 필요하다.

### Interactive

```
User can change what is visualized and how it is visualized.
```

-	인터렉티브 환경은 사용자가 직접 데이터를 선택하고 어떻게 시각화할 것인지 결정을 가능하게 해준다.

### Amplify Cognition

```
Producing tools that help people think better.
This idea is related with cognitive artifacts and distributed cognition.

Some visual representation that helps us store some of the information
rather than having all this information in our mind.
```

-	예를 들어 두개의 큰 수 사이의 곱셈을 암산하는 것보다 종이에 써서 계산하면 쉽게 문제를 해결할 수 있다.
-	이는 중간 단계에서 정보를 저장하기 때문에 우리가 모든 것을 머리 속에서 기억할 필요 없기 때문이다.
-	시각적 표현을 통해서도 이러한 경험을 가능하게 할 수 있다.

Why visualize data?
-------------------

Because data is an abstract representation of some reality or some phenomena we are interested in. In general, people who are using visualization, come with some pre-existing knowledge and some goal related to better understanding some phenomena.

*[img1] Diagram of Data visualization Process* ![Image of VDpipeline](https://github.com/deepnsoul/TIL/blob/master/infovis/fig/VDpipeline.png)

-	문제는 우리가 관심 있는 데이터가 추상적이라는 것이다.
-	시각화를 이용한다면 가지고 있는 지식과 질문을 통해 어떤 현상에 대해 더 나은 이해가 가능하다.

### Three main purposes of Visualization

-	`Explanatory for communication`

	-	to explain something to somebody else
	-	their is someone who has some message or some idea that needs to be communicated visually through data visualization
	-	[Example of Explanatory Visualization](https://www.nytimes.com/interactive/2017/03/21/climate/how-americans-think-about-climate-change-in-six-maps.html)

-	`Exploratory for analyzing data`

	-	to help person answer questions and generate new hypotheses  
	-	there is a person who needs to extract information out of data and does not really know what the content of this data is
	-	Examples of Exploratory Visualizations Tools: Tableau, R-ggplot2, Python-Matplotlib, Seabon

-	`Comfirmatory for analyzing data`

	-	to check whether hypothesis actually holds in the data
	-	there is person who is using visualization here has some hypothesis or question in mind that needs to be checked out

---

-	시각화의 주요 목적은 크게 세 가지로 구분할 수 있다.
-	Explanatory는 아이디어를 전달하기 위한 `Commnunication` 의 목적을,
-	Exploratory는 질문에 대한 답을 찾고 가설을 세우기 위한 `Analyzing` 의 목적을,
-	마지막으로 Comfirmatory는 실제 데이터 안에서 가설을 확인하기 위한 Exploratory와 같은 목적을 가지고 있다.

### Why use a Graphical Representation

1.	Humans are inherently visual animals, and we are very good at processing visual information.

2.	There are three main ways to communicate information. The first one is `verbally`, the second one is `numerically`, and the third one is `graphically`. How does it differ?

	-	When we commnunicate verbally, we are forced to process this information sequentially.
	-	When we use table, problem is that there is not much to see and perceive.
	-	Contrary to these ways, when observing a chart, we are actually consuming and processing this information in a parallel fashion, all at once. We do not need to go through it sequentially.

3.	Problems with summary statistics

	-	statistics are summaries of information that is contained in the data so that we can communicate the most important information.
	-	The problem though with statistics is that they aggregate information and remove a lot of details.
	-	Anscombe's Quartet is an image that consist of four plots with four diffent datasets ![imamge of anscombe's quartet](https://github.com/deepnsoul/TIL/blob/master/infovis/fig/anscombe.png)
	-	As you can see, these four scatter plots have very different patterns. But when we calculate a number of common statistics on top of these four patterns, we realize that they have exactly the same average.
	-	When we visualize data, we can readily perceive information that is hidden in the statistics.

---

-	첫 번째 이유는 인간은 본성적으로 시각적 동물이기 때문에 시각 정보 처리에 능숙하기 때문이다.

-	다음으로 정보를 전달하는 방법은 verbally, numerically,graphically 세 가지가 있다. verbal 방식은 정보를 순차적으로 처리해야 한다는 문제가, table 방식은 보고 인식할 수 있는 정보가 많지 않다는 문제가 있다.

-	이와 다르게, 차트와 같이 graphical 방식은 우리가 정보에 대해 처리와 인식을 동시에 병행하는 것을 가능하게 해준다.

-	마지막으로 통계는 데이터에 대한 요약 정보를 담고 있는데, 이를 통해 우리는 가장 중요한 정보를 전달할 수 있다. 그러나 통계의 문제점은 통합된 정보만 보여주기 때문에 많은 세부 정보들이 제거된다는 점이다.

-	데이터 시각화를 통해 우리는 통계 뒤에 숨겨진 정보를 잘 인식할 수 있다.

### Why Use Computers to Visualize Data?

1.	The first one is obviously that with a computer, we can visualize a lot of data.
2.	The second reason is that computers allow you to interact with digital graphical representations.
3.	But, there are still people who actually like drawing data with their hands. [Dear Data](http://www.dear-data.com/) by Giorgia Lupi and Stefanie Posavec is a beautiful example.

---

-	데이터 시각화 과정에서 컴퓨터를 이용하면 많은 양의 데이터를 시각화 할 수 있다.
-	또한 인터렉티브한 환경도 구성할 수 있는 점도 큰 장점이다.
-	여전히 손으로 직접 데이터를 시작화하는 프로젝트도 진행되고 있는데, 이를 통해 컴퓨터로 할 수 없는 다른 인사이트를 이끌어낼 수 있다.

### Why Use Interaction?

-	Not all questions can be answered by looking at one single visual representation.
-	Therefore, having a system that can change as we interact with it and helps us answer multiple questions.
-	An interesting area of research in visualization is how to do visualization with other devices and other interaction modes.

---

-	단순히 하나의 시각적 표현은 여러 질문에 대한 답변을 할 수 없다.
-	그러므로, 사용자가 직접 시스템을 변경할 수 있는 인터렉티브한 환경은 다양한 질문에 대한 답변을 가능하게 한다.
-	다양한 디바이스에서 어떻게 인터렉티브 환경을 구성할 것인가? 이 주제는 현재 인터렉티브 분야에서 활발하게 진행되고 있는 연구 중에 하나이다.  

### Assessing the Quality of a Visualization

How do you know that one visualization is better than another? Is that not subjective? **Some visual representations are clearly better** because they are easier to interpret, and easier and faster, and more accurate to read.

*[img2] The pie charts of a world of drugs* ![image of pie charts](https://github.com/deepnsoul/TIL/blob/master/infovis/fig/error.png)

-	If your goal is to represent the trend over time and how they change and intersect, it is not a particularly good representation.
-	We tend to perceive quantity with the area of the segments. But the quantity that the designer here wants to convey is actually represented with the angle of the pies.
-	Another problem is that the angle and the size interfere. So it is very hard to disentangle these two pieces of information.
-	One more problem is that if we want to see how proportions change over time, we have to mentally link these areas across the segments, which are also not aligned, which makes these comparison even harder.

*[img3] The line charts of a world of drugs* ![image of pie charts](https://github.com/deepnsoul/TIL/blob/master/infovis/fig/correct.png)

-	But if I represent exactly the same data with a line chart, observing trend over time and how they relate to each other, how these markets relate to each other, is much easier.
-	So, when you are evaluating, assessing the quality of a visual representation, you have to think first of all, what is the intent, what problem am I try to solve, what information am I trying to convey.
-	And then figure out whether one visual representation is bad at conveying this information than the other.

```
Designing effective visualizations requires two main steps.

The first one is knowing the design space.
The second skill is being able to compare the solutions in an effective way.

```

-	First, being able to create a certain number of alternatives is a crucial skills for visualization design.
-	If you do not know how to do that, it will not be possible for you to actually see different solutions and start assessing them.
-	In addition, You have to be able to predict whether a given visual representation is going to be more effective than another.
-	And how do you do that? There are many ways, but the most important skill is how human perception of graphical representation works.

---

-	만약 파이차트를 그린 목적이 시간에 따른 변화를 보고자 한 것이었다면, 이 방식은 좋은 표현이 아니다.
-	몇 가지 이유가 있는데, - 먼저 우리는 구분된 영역의 크기를 통해 그 양을 인지하는 경향이 있다. 그러나 여기서는 실제로 파이의 각도가 양을 의미한다.  
-	다른 문제는 각도와 크기라는 서로 다른 종류의 정보가 이해를 방해하고 해석하기 어렵게 만든다는 것이다.
-	마지막으로 시간에 따른 변화를 보기 위해서는 한 파이차트에서 구분된 영역을 다른 파이차트와 연결해서 봐야하는데, 서로 떨어져있기 때문에 비교가 어렵다는 것이다.
