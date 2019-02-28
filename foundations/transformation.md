Fundamental Graphs and Data Transformation
==========================================

coursera **[Information Visualization: Foundations](https://www.coursera.org/learn/information-visualization-fundamentals/)** course in week3 by **Enrico Bertini** at New York University Tandon School of Engineering

How to Visualize?
-----------------

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
-	모든 단일 시각적 표현은 테이블의 일부 속성들을 이용해서 만들어지기 때문에, 원하는 문제를 해결할 수 있는 그래프를 만드는데 필요한 정보를 추출하기 위해 데이터 변환이 필요하다.  
-	두 번째 단계는 어떻게 시각화할지를 결정하는 것이다.
-	이는 적절한 시각적 표현을 선택하고 디자인하는 것을 의미하는데, 선택은 이미 존재하는 포맷에서 목적에 맞는 적절한 표현을 선택하는 것을 말한다.
-	디자인은 기존의 포맷이 아닌 현 문제에 대한 새로운 시각적 표현을 만드는 것을 말한다.

### Fundamental Graphs

-	what graphs are available to visualize the combination of attributes that you have.
-	There are the bar chart, the scatter plot, the matrix, the line chart and the symbol map.
	-	widely adopted, effective, useful
	-	solve vey large percentage of vis problems
	-	training ground for more sophisticated graphs
-	The graphs can be described as combinations of two of more attributes.

---

-	속성들의 조합을 시각화 할 수 있는 대표적인 그래프에는 막대그래프, 선그래프, 산점도, 매트릭스, 심볼맵이 있다.
-	이들은 널리 채택되고 효과적이며, 유용하고, 상당한 부분의 시각화 문제를 해결할 수 있다.
-	또한 더 복잡한 그래프를 그리기 이전에 훈련할 수 있는 그래프이다.  
-	일반적으로 둘 이상의 속성의 조합을 통해 그래프가 그려지는데 속성의 조합은 그래프 유형에 따라 차이가 있다.

`Bar chart`

![Image of barchart](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_barchart.png)

-	visualize how a quantity distributes acrros a set of categories.
-	So every bar represents one category and the length of the bar represents a quantity.
-	In this specific example, you have boroughs on the x axis and the count of vehicle collisions on the y axis.

---

-	막대 그래프는 범주에 따라 수량이 어떻게 분포하는지를 시각화한다.
-	따라서, 모든 막대는 하나의 범주를 나타내며, 막대의 길이는 수량을 의미한다.
-	그림의 예시에서는 x축에 자치구를, y축에 차량 충돌 수를 나타내고 있다.

`Line chart`

![Image of linechart](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_linechart.png)

-	visualize how a quantity changes in relation to another quantity(typically time)
-	So in this specific case on the x axis we have time and on the y axis we have the amount of vehicle collisions over time.
-	And as you can see we can identify some trends.

---

-	선 그래프는 한 수량이 다른 수량(일반적으로 시간)에 관련하여 어떻게 변화하는지를 시각화한다.
-	그림의 예시에서는 x축에 시간을, y축에는 차량 충돌의 양을 나타내고 있다.
-	이러한 선 그래프를 통해 우리는 몇 가지 추세를 확인할 수 있다.

`Scatter plot`

![Image of scatterplot](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_scatterplot.png)

-	visualize how a quantity relate to another quantity
-	In this specific scatter plot from a food products dataset on the x axis we have amount of calories and on the y axis we have amount of carbohydrates.
-	So scatter plot visualizes relationship between a quantity and quantity.  

---

-	산점도는 한 수량과 다른 수량의 관계가 어떠한지를 시각화한다.
-	식품에 관한 데이터 세트를 나타내는 그림의 예시에서는 x축은 칼로리를, y축은 탄수화물의 양을 나타내고 있다.
-	즉, 산점도는 수량과 수량 사이의 관계를 시각화한다.

`Matrix`

![Image of matrix](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_matrix.png)

-	visualize how a quantity distributes across two categories
-	So we have one categorical attribute on the y axis and another categorical attributes on the other axis.
-	here what they put in this table is vehicle one and vehicle two in rows and columns and what you see within each cell is again the number of collisions that happen in the combination of these two vehicle types.

---

-	매트릭스는 두 개의 범주에 관련한 한 수량이 어떻게 분포하는지를 시각화한다.

-	따라서, y축에 하나의 범주적 속성을, 다른 축에 다른 범주적 속성을 가지게 된다.

-	그림의 예시에서는 차량 1과 차량 2를 행과 열로 구분하고, 각 셀 안에서는 두 가지 유형의 차량의 조합으로 발생되는 충돌 수를 나타내고 있다.

`Symbol map`

![Image of matrix](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_symbolmap.png)

-	visualize how a quantity distributes across two spatial coordinates
-	In this specific case, every single dot represents one zip code  
-	So every dot is a zip code and the size of this symbol represents how many collisions happened in the area represented by the zip code.

---

-	심볼맵은 두 공간 좌표에 관련한 한 수량이 어떻게 분포하는지를 시각화한다.
-	그림의 예시에서는 지도 상의 모든 개별 점은 우편번호를, 점(심볼)의 크기는 우편 변호 지역에서 충돌이 발생한 횟수를 나타내고 있다.  

*[img6] Summary of fundamental chats* ![Image of basic charts ](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/basic_charts.png)

This is a summary of the graphs that I have just shown you and what kind of information, what kind of attributes, or combination of attributes can be represented with these graphs

---

-	요약 그림에서는 다섯 개의 그래프가 각 각 어떠한 속성의 조합을 통해 생성될 수 있는지를 보여준다.  

### Alternate Representations

#### #. day 12, 190112

It is possible to create different representation of the same data. Being able to think about alternative visual representations for the same information is one of the most important skills because it is useful once you have a number of alternatives in mind to be able to reason about which one is the most appropriate for your goal.

---

동일한 데이터에 대해서 다양한 시각적 표현이 가능한데, 같은 정보에 대해서 대안적인 시각적 표현을 생각해내는 것은 중요한 기술 중 하나이다. 가장 적합한 시각적 표현을 찾는 목표를 이루기 위해서 여러 가지 대안을 비교하는 것이 유용하기 때문이다.

`Bar graph alternatives`

![Image of bar_alternatives](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/bar_alternatives.png)

-	*dot plot*
-	![Image of bar-alt_dotplot](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/bar-alt_dotplot.png)

	-	we can use a simple dot.
	-	but, it is hard for us typically when we see a cloud of dot like this one.
	-	if we draw a little line like this one, all in a sudden we go back to interpreting this chart very similarly to the way we interpret a bar chart.

---

-	막대 그래프의 대안으로 단순히 점을 이용할 수 있다.
-	그러나, 점만 찍어서는 어떤 범주에 대한 값 인지를 알아보기 어렵기 때문에 그림에서와 같이 범주와 선을 연결한다면, 막대 그래프와 유사하게 이해가 가능하다.

-	line chart

	-	we can connect these dots with lines.
	-	the problem is this that the line chart tends to communicate to the reader the idea that these values are ordered.
	-	Not only that, a line chart creates a very distinctive pattern, and we tend to interpret this pattern as meaningful.
	-	But, when we have categorical information or categorical attribute on the x-axis, this pattern is not really meaningful, and these data items are not really ordered.

---

-	점들을 선으로 연결하여 선 그래프를 만들 수 있는데, 문제는 이러한 선 그래프가 값들 간의 순서가 있다는 정보를 내포하고 있다는 것이다.
-	또한, 선 그래프는 구별되는 패턴을 생성하기 때문에, 패턴을 의미를 부여하게 된다.
-	그러나 실제로 x축이 범주형 속성이라면, 이러한 패턴은 의미가 없으며, 값에 대한 순서도 없다.

-	*bubble chart*

-	![Image of bar-alt_bubbles](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/bar-alt_bubbles.png)

	-	the area of the bubbles represents the value that corresponds to each category.
	-	the problem is that it is much less common to represent the data in this way. So, your reader to be less comfortable with this visual representation.
	-	the second problem as we will see later on in the course is that area size is not as effective in terms of communicating quantitative information as comparing the length of two bars.

---

-	버블 그래프에서 버블 영역은 각 각의 범주에 대응하는 값을 나타낸다.
-	문제는 이러한 방식으로 데이터를 표현하는 것이 일반적이지 않기 때문에 독자들이 익숙하지 않을 수 있다.
-	또한 버블의 면적 크기가 두 막대를 길이를 비교하는 것 만큼 양적 정보를 전달하는데 효과적이지 않다는 것이다.  

`Scatter plot alternatives`

![Image of scatter-alt_slope](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/scatter-alt_slope.png)

-	slope chart
	-	this graph is called the slope chart.
	-	we have two parallel axes. Every item in the dataset can be represented by a line connecting the two values that are in the two axes.
	-	What the slope chart is useful for is to see when the values are going in one direction or in the other direction.
	-	in these example, on the left hand side axes, we have the proportion between wins and losses of each team and on the other axis on the right hand side, you have the amount that has been spent by the team to hire the players.
	-	so, here what you see is that the slopes that go up mean teams that are not performing particularly well but spend a lot of money.

---

-	경사(slope) 그래프는 산점도와는 다르게 두 개 축이 서로 평행하며, 두 축에 있는 값을 연결하는 선으로 나타낼 수 있다.
-	경사 그래프는 값이 언제 올라가고 내려가는지 확인하는데 유용하다.
-	그림에서 왼쪽 축은 팀의 승리와 패배 점수의 비율이고, 오른쪽 축은 팀이 선수를 고용하는데 소비한 비용이다.
-	올라가는 경사를 가진 팀이 돈을 많이 쓴 것에 비해 시합 결과가 좋지 않다는 것을 의미하며, 내려가는 경사는 그 반대를 의미한다.  

`Line graph alternatives`

![Image of line_alternatives](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/line_alternatives.png)

-	bar chart

	-	in the one that you see on the right, in place of lines, we have bars like in a bar chart, which is not as effective as the line chart to represent the actual trend, but it is useful in case you want to read the values, every single value accurately.

-	area chart

	-	the next one is the area chart, which is basically a version of the line chart where the area below the line is completely filled up.

-	simple dots

	-	the last one is one where we use just the simple dots.
	-	but the problem with this one is that we cannot really trace the line and we cannot really see the trend.

---

-	선 그래프의 대안으로 세 가지를 생각해볼 수 있다.
-	먼저, 오른쪽의 막대 그래프는 추세를 확인하는데에는 효과적이지 않지만, 각 각의 값 자체를 보는데는 유용하다.
-	면적 그래프는, 아래 영역이 완전히 채워지는 선 그래프를 말한다.
-	마지막으로 단순한 점을 사용할 수 있는데, 실제로는 점들을 추적하기 어렵기 때문에 추세를 제대로 파악할 수 없다.

`Matrix alternatives`

![Image of def_matrix](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/def_matrix.png)

-	The matrix accommodates two categorical attributes, which are mapped into a few rows and a few columns.
-	In this case, we have two rows and three columns. The values that are associated to the intersection of these categories are represented like the area of a symbol.
-	In this case, the area of a square.
-	These are the kind of information that you have to use to imagine different alternative visual representations for the matrix.

---

-	매트릭스는 두 범주형 속성을 가지며, 행과 열로의 매핑을 통해 표현된다.  
-	그림의 경우, 두 개의 행과 세 개의 열이 있고, 두 개의 범주의 교차에 대한 값이 영역으로 표시된다. 여기서는 정사각형으로 표현하고 있다.
-	이러한 정보를 가지고 매트릭스에 대한 대안적인 시각적 표현을 생성할 수 있다.  

![Image of matrix_alternatives](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/matrix_alternatives.png)

-	stack bar chart

	-	the idea is that one way to arrange two categories is to use the rows for one of the categories
	-	every bar that represents each of the categories is split in a number of smaller bars, colored bars, where every color represents the values of the other category.
	-	but, it is pretty hard to see the distribution of the values across the two categories.

-	bar graph

	-	a graph where the two categories are nested.
	-	we have rows for each categories.
	-	within each category nested, we have the other categories.
	-	but one problem here is that it does not scale visually as easily as the matrix representation.

---

-	매트릭스에 대한 대안적인 시각적 표현으로 누적막대 그래프와 막대 그래프를 사용할 수 있다.
-	누적막대 그래프는 여러 범주를 한 행 또는 열로 표현한다.
-	따라서 각 범주를 나타내는 막대는 여러 개의 작은 막대로 나뉘며, 색상은 다른 범주의 값을 의미한다.
-	그러나, 누적막대 그래프는 개별 범주가 아닌 범주에 걸쳐 값의 분포를 보는 것이 꽤 어렵다.
-	다음 방법으로 두 개의 범주를 중첩하여 막대 그래프로 표현할 수 있다.
-	각 각의 범주를 행으로 나누고, 행 안에 세부 범주에 대한 값을 막대 그래프로 나타낼 수 있다.
-	그러나 이는 막대의 길이가 들쭉날쭉하여 매트릭스처럼 시각적으로 표현을 확장하기에 어려움이 있다.  

`Symbol map alternatives`

![Image of def_symbolmap](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/def_symbol.png)

-	We have two quantities that represent the location.
-	x1, y1, x2, y2, and so on, and each one is represented with a small symbol and the size is proportional to the quantity.

---

-	심볼맵은 위치를 나타내는 두 개의 값(x, y)을 지도에 기호로 나타내는데, 이때 기호의 크기는 해당 위치의 값의 비율을 의미한다.

![Image of symbol_alternatives](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/symbol_alternatives.png)

-	bar chart
	-	get rid of the map completely and just create a list of locations, which in this case is a list of zip codes.
	-	And for every zip code, we represent the value with a bar.
	-	Every single zip code is a category and every bar is associated to a zip code and as a length that represents the quantity that is associated to the zip code.

---

-	심볼맵을 막대 그래프로 나타낼 수 있는데, 먼저 지도는 제거하고, 위치 목록을 우편번호를 이용하여 만들 수 있다.
-	즉, 개별 우편 번호는 범주가 되며, 모든 막대의 길이는 우편번호와 관련한 값을 의미한다.

### Going Beyond Two Attributes

#### #. day 13, 190113

If you have additional attributes and you want to be able to introduce in the representation, there are several designs which is belonging to each charts.

---

-	추가적인 속성을 기존의 그래프에 추가하기 위한 몇 가지 방법이 있다.

`Bar charts`

![Image of bar_overtwo](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/bar_overtwo.png)

In the vehicle collision data, we have vehicle type, main cause for the accident, and for each combination of these two categories, how many accidents or how many people injured we have. how do we represent these information with a bar chart? There are two main designs.

---

-	그림의 예시는 차랑 충돌 데이터에서, 차량 유형과 사고의 주요 원인, 이 두 범주의 조합에 대해서 얼마나 많은 사고가 발생했는지를 막대 그래프의 두 가지 디자인으로 나타낸 것이다.

-	stacked

	-	we have as many bars as the number of categories that are included in the first categorical attribute and as many segments within each bar as the values that are in the other categorical attribute.
	-	In this case, we have vehicle types represented by the three bars that you see in the stacked bar chart, and the main causes for collisions represented by the five colored.
	-	the stacked bar graph is very good when your main question is regarding the proportion.

-	grouped

	-	one categorical attribute is mapped to the bar chart and this bar chart is repeated as many times as the number of categories that you have in the other categorical attribute. -the grouped bar chart is better when the goal is to compare every single value one to another.

---

-	먼저 누적막대 그래프는 첫 번째 속성을 범주를 여러 막대로 표현하고, 다른 나머지 속성을 각 각의 막대 내부에 구분을 두어 나타낸다.
-	이번 예시의 경우 차량 유형을 3 개의 막대로, 충돌의 주요 원인을 5 가지 색상으로 막대 내부를 구분하였다.
-	주요 질문이 비율에 관한 것이라면 누적 막대 그래프가 유용하다.
-	다음으로 그룹 막대 그래프는 첫 번째 속성의 범주들을 그룹 막대 그래프로 매핑하고, 다른 속성의 범주 수 만큼 그룹 막대 그래프를 반복하여 나타낸다.
-	개별 값을 비교하려는 경우 그룹 막대 그래프가 유용하다.

`Line charts`

![Image of line_overtwo](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/line_overtwo.png)

In the vehicle collision data, we have on the x-axis, time, year of the date, and on the y-axis we have number of collisions. we have an additional attribute which is the borough.

---

-	이번 그림의 예시 또한 차랑 충돌 데이터에서, x축은 시간, 년도를, y축은 충돌의 수를 보여준다. 추가적인 속성인 자치구를 그래프에 나타내기 위한 세 가지의 디자인을 생각해볼 수 있다.

-	separate lines

	-	each one representing one borough
	-	This is very good because since we have the lines represented in the same space, it is easy to compare their values.

-	every single line is represented in a separate line chart.

-	it is a sort of series of line charts one next to the other, one above or below the other.

-	stacked area chart

	-	the values across the categories are stacked one on top of the other.
	-	these stacked area chart is good if the only question that you have is how does the proportion of these values change over time
	-	but, it is not good to compare the values of these categories over time because the pattern that you see in the lines is affected by the shape of the line that is below the one that you are observing.

---

-	먼저, 색상으로 구분된 선 그래프인데, 각 각의 선은 한 자치구를 의미한다.
-	이러한 형태의 디자인은 같은 공간에 모든 선들을 나타내기 그들 간의 값을 비교하기 쉽다.
-	다음으로 개별 선마다 구분하여 그래프를 그리는 방식인데, 개별적인 선 그래프를 아래로 나열해서 볼 수 있다.
-	마지막으로 누적 영역 그래프는 개별 범주의 값을 누적하여 위로 쌓아 나타내는 방식이다. 이러한 그래프는 값의 비율이 시간에 따라 어떻게 변하는지 알아보고자 할 때만 유용하다.
-	다만, 시간 변화에 따른 범주 사이의 값을 비교하는 경우에는 모든 선의 형태가 바로 아래에 있는 선의 형태에 영향을 받기 때문에 이 방식이 효과적이지 않다.

#### #. day 14, 190114

`Scatter plots`

![Image of scatter_3attri](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/scatter_3attri.png)

here is another scatter plot having third attribute. That encodes information about a number of categories, each category, one color.

---

-	그림은 두 개의 속성을 가진 산점도에 하나의 속성을 색상으로 표현하여 총 세 개의 속성을 나타낸 산점도이다.  

![Image of scatter_4attri](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/scatter_4attri.png)

A scatter plot can encode up to four attributes. So in this case, we have exactly the same scatter plot, which is encoding one attribute on the X-axis, one on the Y-axis, now another one with color, and even another one with the size of the dots or bubbles.

---

-	이번 그림은 앞서 세 개의 속성을 표현한 산점도에 하나의 속성을 더 추가하여 점이나 버블의 크기를 통해 나타낸 산점도이다.
-	산점도에서는 최대 네 개까지의 속성을 인코딩할 수 있으며, 그 이상은 인코딩된 정보를 이해하기 어려워 질 수 있다.

![Image of scatter_facet](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/scatter_facet.png)

We can do is to create a replica of the same scatter plot, where every single one contains only the data of one of the categories. They all come from the original scatter plot, and each one shows only the data that belongs to one of the categories that you see in the region on the right.

This is a very general purpose technique, that is called faceting, and visualization method that you see here is also sometimes called small multiples.

---

-	그림은 색상으로 나누어진 한 범주의 항목들에 대해서 개별 산점도로 분할하여 나타내었다. 이렇게 한 범주의 항목을 나누어 표현하는 시각화 방법을 faceting 또는 small multiples라고 부른다.

-	`Faceting`

	-	select one categorical/ordinal attribute
	-	create as many sets as the number of values
	-	create one plot for each value
	-	Faceting can be applied to any graph.
	-	![Image of map_facet](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/map_facet.png)
	-	Faceting with maps: I have data about the city of New York, and I split this information into different categories, and each map represents the data coming only from one of the categories.
	-	![Image of line_facet](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/line_facet.png)
	-	Faceting with line charts: I have one, two, three, four, five different categories of things that are changing over time, and rather than putting them all together in one graph overlapping, I create one graph for each of them.
	-	this is a very general purpose technique, and it is useful especially when you have too many categories to show at once. you do not have an easy way to put all these categories together in one single plot.
	-	you can just split them into a number of plots, and create what is called a small multiples presentation.

---

-	faceting은 세 가지 단계를 통해 진행될 수 있는데,
-	먼저 하나의 범주형 속성을 정한 후 범수의 항목 별 값의 집합을 생성한다.
-	다음으로 각 각의 값의 숫자 만큼 그래프를 그린다.
-	faceting은 산점도 이외에도 모든 그래프에서 적용할 수 있다.
-	맵 그래프를 faceting 한 그림의 예시를 보면, 뉴욕시에 대한 데이터이고, 하나의 범주 대해 개별적으로 항목을 분리하여 표현하였다.
-	선 그래프를 faceting 한 그림의 예시는 한 범주의 다섯 개의 항목들에 대해 각 각의 그래프로 나타낸 것이다.
-	faceting 방법은 한 범주의 항목들이 너무 많은 경우 유용하다. 모든 항목들을 하나의 단일 그래프에 표현하기는 쉽지 않다.
-	따라서 여러 그래프로 분할하여 small multiples 방법으로 나타낼 수 있다.

### Data Transformation

#### #. day 16, 190116

We have two steps of data visualization. Now, we are going back to the first step, in trying to look into more details what this means.

---

데이터를 시각화 과정은 크게 두 단계 select and transform와 choose/design representation 로 구분된다. 여기서는 첫 번째 단계인 select and transform 을 자세히 살펴보려 한다.

-	`selection: select from the table the attributes needed for the visualization`
	-	ex1) selecting three attributes and using a scatter plot ![Image of selecting_scatter](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/selecting_scatter.png)
	-	In the food data set: visualize the relationship between carbohydrates and calories see how it is affected food category.
	-	We are starting from a large data table with lots of attributes, and selecting three attributes out of them, which are those attributes that we need in order to answer these questions.
	-	ex2) selectung two attributes and using a bar chart ![Image of selecting_bar1](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/selecting_bar1.png)  
	-	see how the average amount of calories distributes across food category.
	-	to do that, I have to select the food category and the amount of calories. every single bar represents one fruit category, and the height of the bar represents the average amount of calories.
	-	ex) an intermediate step ![Image of selecting_interme](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/selecting_interme.png)  
	-	but an intermediate aggregation step is necessary to answer this question. I need to aggregate information across all products, in order to calculate the average amount for every single category.

---

-	먼저 selection은 테이블에서 시각화를 위해 필요한 속성을 선택하는 과정을 말한다.
-	그림의 예시는 식품 데이터 세트에서 탄수화물과 칼로리 간의 관계를 식품의 범주에 따라 어떻게 차이가 있는지 살펴보기 위해서 산점도로 시각화한 것이다.
-	즉, 테이블의 많은 속성들 중 질문에 대한 답을 찾기 위해 세 개의 속성들을 선택하였다.
-	다른 예시는 같은 식품 데이터 세트에서 칼로리의 평균이 식품의 범주에 따라 어떠한 분포를 가지는지 파악하기 위해서 막대 그래프로 시각화한 것이다.
-	테이블에서 식품 유형과 칼로리의 양 두 개의 속성을 선택한 후 막대 그래프를 생성할 수 있고, 막대 그래프의 단일 막대는 과일의 범주를 나타나며, 높이는 평균 칼로리 양을 의미한다.
-	그러나 이러한 막대 그래프를 생성하기 위해서는 데이터 선택 외의 단일 과일 범주에 대해서 평균 칼로리 양을 각 각 계산하는 그림과 같은 중간 단계가 필요하다.

-	`the intermediate step(transfomation)` ![Image of transform_interme](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/transform_interme.png)

-	virtually all graphs require selection many require aggregation or other transformations.

	-	Starting from the original table, first I have to select two columns, but I also have to aggregate these two columns together to generate the information that I need.
	-	In this case, I need to aggregate all the categories together, and calculate the average across all food products that belong to each of these categories.
	-	common aggregation functions: SUM, MAX, MIN, AVERAGE, MEDIAN, STDDEV

---

-	실제로 모든 그래프는 selection과 총합 또는 다른 transformation들을 필요로 한다.
-	그림의 예시처럼 먼저 두 개의 열을 선택하고, 두 개의 열을 aggregation 하여 우리가 필요한 정보를 생성할 필요가 있다.
-	여기에서는 개별 범주들끼리 분류하고 평균을 구하였다. 일반적으로 aggregation 기능은 합계, 최대값, 최소값, 평균, 중앙값, 표준편차 등이 있다.  

### Common / Useful Data Transformations

#### #. day 18, 190118

-	Time and date: a hierarchical structure

	-	Aggregation by: seconds, minutes, hours, day, week, month, year(time resolutions)
	-	*ex) visual presentations at different levels of resolution* ![Image of time_resolutions](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/time_resolutions.png)
	-	using different resolutions has an impact on the way this information is visualized.
	-	There is never one single resolution that is optimal. It depends on the specific question that you have and on the specific project you’re working on.

-	Spatial

	-	Aggregation by: zip code, county, state

-	Geo coding and decoding

	-	Name -> Geo-coordinates | Geo-coordinates -> Name

---

-	데이터의 유형에 따라 자주 사용되는 aggregations가 있다.
-	먼저, 시간과 날짜는 위계적인 구조로, 각 각 초, 분, 시 | 날짜, 주, 월, 년 의 시간 해상도를 가진다.
-	그리고 그림의 예시처럼 어떤 해상도(resolution) 수준을 선택했는지에 따라 시각화 형태가 달라진다.  
-	최적의 해상도는 존재하지 않으며, 진행하고 있는 프로젝트의 특정 질문에 맞는 해상도 선택해야한다.
-	공간 데이터는 일반적으로 우편번호, 자치주, 주 의 해상도를 가진다.
-	지역 데이터의 경우에는 보통 지역의 이름을 위도 경도와 같은 지리적 정보로 코딩하거나, 반대로 디코딩하는 두 가지의 해상도를 가진다.

#### #. day 19, 190119

-	quantitative to ordinal through binning

	-	binning: you take the quantities, and you bin them into a number of categories, and then you sort them according to their values.
	-	*an example of binning* ![Image of quan_to_ordi](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/quan_to_ordi.png)
	-	I have an attribute that is called profit, the amount of profit that comes from each sale. So there are lots of different values
	-	But if I want to transform this attribute into a discrete one, into an ordinal one, what I can do is just to aggregate these values into a number of bins.
	-	Going from one range to another range, and just create one single category for each one.

---

-	양적 자료를 순서 자료로 바꿀 수 있는데, 범주를 임의적으로 만들어서 값에 따라 분류하는 binning을 통하여 데이터 변환을 할 수 있다.
-	그림의 그래프는 각 각의 판매에서 오는 수익을 표현하고 있으며, 만약 개별 판매의 값을 하나씩 다루면 엄청나게 다양한 값이 x축에 나타나게 된다.  
-	따라서 개별 판매라는 다양한 값을 몇 개의 범주로 분류하여 나타내었다. 즉, 특정 범위의 값을 하나의 범주에 포함시켜 양적 자료를 이산적인 순서 자료로 변환하였다.

-	rescaling / re-expression a given quantitative attribute, typically through normalization.

	-	normalization: if your attribute has a given minimum and maximum value, you can represent the same range using a different scale. ex) [-1,+1]
	-	*percentage case* ![Image of resc_perc](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/resc_perc.png)
	-	on the left is expressing information in terms of counts, and the one on the right is expressing information in terms of percentages.
	-	this analysis is to see how different cuisine types, how the distribution of grades changes across cuisine types.
	-	since there are different number of restaurants across cuisine types, if I use only raw numbers, which is on the left chart, I cannot really compare across different cuisines.
	-	On the right chart, I am re-expressing the same information in terms of percentages, so I no longer have the problem.
	-	There are many situations where calculating percentages makes comparison between values easier.
	-	distance from reference:ex) you have all the quantities in an attribute, you calculate the average value and you want to re-express them in terms of distance from the average value.

---

-	양적 속성의 데이터를 재배정 또는 재표현하기도 하는데, 이는 정규화를 통해 데이터 변환이 가능하다.
-	정규화는 속성이 최대값, 최소값을 가질 때, 다른 기준(척도)을 이용하여 같은 범위를 나타내는 방법이다. 예를 들어 범위가 넓게 퍼져있는 음수, 양수 값을 [-1,+1] 기준으로 재배정 할 수 있다.  
-	그림의 그래프는 다양한 요리 종류에 따라 평가가 어떻게 변하는지를 나타내고 있는데, 왼쪽의 y축은 빈도수를 오른쪽은 백분률로 표현하고 있다.
-	문제는 식당에 따라 요리 종류를 나타내고 있기 때문에, 왼쪽과 같이 평가 점수로 표현하면 식당 별로 비교하기가 쉽지 않다.
-	따라서 오른쪽과 같이 정보를 백분율로 재표현하여 문제를 해결할 수 있는데, 이와 같이 비율을 계산하면 값을 쉽게 비교할 수 있는 경우가 많이 있다.  
-	또다른 재표현 방식은 특정 값에 대해 거리를 이용하는 것인데, 예를 들어 속성이 모든 값을 가지고 있으면 평균값을 계산하고 평균값과의 거리를 기준으로 다시 표현할 수 있다.

`Data transformation part of the design process`

-	Most project require you to think creatively about how transformation may lead to better communication and understanding.

`Role of transformation in visualization`

-	Visualizing data is not only about how to visualize data but also what information to visualize. It is up to you to produce the right information needed for your problem.

---

-	정리하자면, 데이터 변환도 디자인 프로세트의 한 부분이라고 볼 수 있다.
-	대부분의 프로젝트에서 더 나은 커뮤니케이션과 이해를 가능하게 하는 창의적인 데이터 변환을 요구한다.
-	데이터 시각화는 단지 어떻게 데이터를 시각화할지에 대한 것만이 아니라, 어떤 정보를 시각화할지를 고민해야되며, 문제를 해결하기 위해 필요한 올바른 정보를 만들어내는 역량이 중요하다.
