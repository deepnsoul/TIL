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

-	물리적으로 보이지 않는 추상적인 데이터를 어떻게 표현할까? 예를 들어 시간이라면 어떻게 표현되어야 가장 적합할지 고민이 필요하다.

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

-	예를 들어 두개의 큰 수 사이의 곱셈을 암산하는 것보다 종이에 써서 계산하면 쉽게 문제를 해결할 수 있는데, 이는 중간 단계에서 정보를 저장하기 때문에 우리가 모든 것을 머리 속에서 기억할 필요 없기 때문이다. 시각적 표현을 통해서도 이러한 경험을 가능하게 할 수 있다.

Why visualize data?
-------------------

Because data is an abstract representation of some reality or some phenomena we are interested in. In general, people who are using visualization, come with some pre-existing knowledge and some goal related to better understanding some phenomena.

*[img1] Diagram of Data visualization Process* ![Image of VDpipeline](https://github.com/deepnsoul/TIL/blob/master/infovis/fig/VDpipeline.png)

-	문제는 우리가 관심 있는 데이터가 추상적이라는 것이다. 시각화를 이용한다면 가지고 있는 지식과 질문을 통해 어떤 현상에 대해 더 나은 이해가 가능하다.

### Three main purposes of Visualization

시각화의 주요 목적은 크게 세 가지로 구분할 수 있다. Explanatory는 아이디어를 전달하기 위한 `Commnunication` 의 목적을, Exploratory는 질문에 대한 답을 찾고 가설을 세우기 위한 `Analyzing` 의 목적을, 마지막으로 Comfirmatory는 실제 데이터 안에서 가설을 확인하기 위한 Exploratory와 비슷한 목적을 가지고 있다.

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
