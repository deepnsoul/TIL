Fundamental Graphs and Data Transformation
==========================================

coursera **[Information Visualization: Foundations](https://www.coursera.org/learn/information-visualization-fundamentals/)** course in week3 by **Enrico Bertini** at New York University Tandon School of Engineering

How to Visualize?
-----------------

#### #. day 08, 190108

> How do I visualize this? How do I go from data to a visual representation that helps you answer some important questions that you have about the data? we can break the problem down into two steps.

1.	`Decide what to visualize`

	-	selecting and transforming the data
	-	every single representation is typically created by using a very small subset of the attributes that you have in the original table.
	-	data needs to be transformed to extract the information that you need in order to create the chart that solves the problem that you want to solve.

2.	`deciding how to visualize it`

	-	choosing or designing an appropriate representation
	-	choosing is exclusively about selecting an existing format that is appropriate for the goal that you have in mind.
	-	designing is more in general trying to create a novel representation for the problem that you have.

---

-	데이터로부터 질문에 대한 답을 얻기 위해서 어떻게 시각화를 해야할까?
-	이 문제를 해결하기 위해 두 단계로 진행할 수 있다.
-	첫 번째는 무엇을 시각화할지 결정하는 것인데, 이는 데이터를 선택하고 변형하는 과정을 의미한다.
-	모든 단일 시각적 표현은 테이블의 일부 속성들을 이용해서 만들어지기 때문에, 원하는 문제를 해결할 수 있는 차트를 만드는데 필요한 정보를 추출하기 위해 데이터 변환이 필요하다.  
-	두 번째 단계는 어떻게 시각화할지를 결정하는 것이다.
-	이는 적절한 시각적 표현을 선택하고 디자인하는 것을 의미하는데, 선택은 이미 존재하는 포맷에서 목적에 맞는 적절한 표현을 선택하는 것을 말한다.
-	디자인은 기존의 포맷이 아닌 현 문제에 대한 새로운 시각적 표현을 만드는 것을 말한다.

### Fundamental Graphs

#### #. day 11, 190111

-	what graphs are available to visualize the combination of attributes that you have.
-	There are the bar chart, the scatter plot, the matrix, the line chart and the symbol map.
	-	widely adopted, effective, useful
	-	solve vey large percentage of vis problems
	-	training ground for more sophisticated graphs
-	The graphs can be described as combinations of two of more attributes.

---

-	속성들의 조합을 시각화 할 수 있는 대표적인 그래프에는 막대차트, 선차트, 산점도, 매트릭스, 심볼맵이 있다.
-	이들은 널리 채택되고 효과적이며, 유용하고, 상당한 부분의 시각화 문제를 해결할 수 있다.
-	또한 더 복잡한 그래프를 그리기 이전에 훈련할 수 있는 그래프이다.  
-	일반적으로 둘 이상의 속성의 조합을 통해 그래프가 그려지는데 속성의 조합은 그래프 유형에 따라 차이가 있다.

-	`Bar chart`

	-	visualize how a quantity distributes acrros a set of categories.
	-	So every bar represents one category and the length of the bar represents a quantity.
	-	In this specific example, you have boroughs on the x axis and the count of vehicle collisions on the y axis.

*[img1] Bar chart* ![Image of barchart](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_barchart.png)

---

-	막대 차트는 범주에 따라 수량이 어떻게 분포하는지를 시각화한다.
-	따라서, 모든 막대는 하나의 범주를 나타내며, 막대의 길이는 수량을 의미한다.
-	그림의 예시에서는 x축에 자치구를, y축에 차량 충돌 수를 나타내고 있다.

*[img2] Line chart* ![Image of linechart](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_linechart.png)

-	Line chart
	-	visualize how a quantity changes in relation to another quantity(typically time)
	-	So in this specific case on the x axis we have time and on the y axis we have the amount of vehicle collisions over time.
	-	And as you can see we can identify some trends.

---

-	선 차트는 한 수량이 다른 수량(일반적으로 시간)에 관련하여 어떻게 변화하는지를 시각화한다.
-	그림의 예시에서는 x축에 시간을, y축에는 차량 충돌의 양을 나타내고 있다.
-	이러한 선 차트를 통해 우리는 몇 가지 추세를 확인할 수 있다.

*[img3] Scatter plot* ![Image of scatterplot](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_scatter.png)

-	Scatter plot
	-	visualize how a quantity relate to another quantity
	-	In this specific scatter plot from a food products dataset on the x axis we have amount of calories and on the y axis we have amount of carbohydrates.
	-	So scatter plot visualizes relationship between a quantity and quantity.  

---

-	산점도는 한 수량과 다른 수량의 관계가 어떠한지를 시각화한다.
-	식품에 관한 데이터 세트를 나타내는 그림의 예시에서는 x축은 칼로리를, y축은 탄수화물의 양을 나타내고 있다.
-	즉, 산점도는 수량과 수량 사이의 관계를 시각화한다.

*[img4] Matrix* ![Image of matrix](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_matrix.png)

-	Matrix
	-	visualize how a quantity distributes across two categories
	-	So we have one categorical attribute on the y axis and another categorical attributes on the other axis.
	-	here what they put in this table is vehicle one and vehicle two in rows and columns and what you see within each cell is again the number of collisions that happen in the combination of these two vehicle types.

---

-	매트릭스는 두 개의 범주에 관련한 한 수량이 어떻게 분포하는지를 시각화한다.

-	따라서, y축에 하나의 범주적 속성을, 다른 축에 다른 범주적 속성을 가지게 된다.

-	그림의 예시에서는 차량 1과 차량 2를 행과 열로 구분하고, 각 셀 안에서는 두 가지 유형의 차량의 조합으로 발생되는 충돌 수를 나타내고 있다.

*[img5] Symbol map* ![Image of matrix](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_symbolmap.png)

-	Symbol map
	-	visualize how a quantity distributes across two spatial coordinates
	-	In this specific case, every single dot represents one zip code  
	-	So every dot is a zip code and the size of this symbol represents how many collisions happened in the area represented by the zip code.

---

-	심볼맵은 두 공간 좌표에 관련한 한 수량이 어떻게 분포하는지를 시각화한다.
-	그림의 예시에서는 지도 상의 모든 개별 점은 우편번호를, 점(심볼)의 크기는 우편 변호 지역에서 충돌이 발생한 횟수를 나타내고 있다.  

*[img6] Summary of fundamental chats* ![Image of basic charts ](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_charts.png)

This is a summary of the graphs that I've just shown you and what kind of information, what kind of attributes, or combination of attributes can be represented with these graphs

---

-	요약 그림에서는 다섯 개의 그래프가 각 각 어떠한 속성의 조합을 통해 생성될 수 있는지를 보여준다.  
