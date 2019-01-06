Data Abstraction
================

coursera **[Information Visualization: Foundations](https://www.coursera.org/learn/information-visualization-fundamentals/)** course in week2 by **Enrico Bertini** at New York University Tandon School of Engineering

What is the role data plays in the visualization process?
---------------------------------------------------------

*[img1] Three main stages of data processing* ![Image of dataprocess](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/dataprocess.png)

1.	`Collection`: create data
2.	`Transformations`: to convert the data into a format or configuration that is necessary to transform them into visual representations
3.	`Visual Encoding`: how to transform this data into a visual form

---

-	시각화 과정에서 데이터는 어떠한 역할을 할까? 데이터가 활용되는 단계는 세 가지로 나눌 수 있다.
-	데이터는 각 각 수집, 변형, 시각적 인코딩 과정을 거치는데,
-	변형은 원본 데이터를 바로 시각화 할 수 없는 경우, 원본 데이터로부터 시각화가 가능한 형태로 데이터를 새롭게 구성하는 과정을 말한다.
-	시각적 인코딩은 데이터를 시각적 형태로 바꾸는 과정인데, 특정 데이터에 대해 어떠한 시각적 표현이 적절한지 어떻게 알 수 있을까?
-	이러한 문제를 해결하기 위해 데이터 추상(Data Abstraction) 개념을 이용할 수 있다.  

What is Data Abstraction?
-------------------------

> " Data abstraction is a method that describe data in ways that help you decide what operations(transformations) and encoding methods are available and appropriate."

-	데이터 추상은 데이터를 변형하고 적합한 인코딩 방법을 찾는 과정을 돕기 위해 데이터를 표현하는 방식이다.  

> " Abstracting away from the domain the characteristics that are useful to decide what visual representations are available and appropriate"

-	또한 데이터 추상은 서로 다른 영역의 데이터이지만 동일하게 적용될 수 있는 적절한 시각적 표현을 찾는데 도움이 된다.

---

-	정리하자면, 우리가 데이터를 수집한 뒤 데이터를 어떻게 시각화할지 고민하기에 앞서, **수집된 데이터가 어떤 종류의 데이터인 먼저 파악** 해야 한다.
-	데이터를 파악하는 과정에서 데이터 추상이 이용되고, 이는 우리가 데이터를 알맞게 변형하여 적절한 시각적 표현을 선택할 수 있도록 도울 것이다.

### Dataset Types

```
Every dataset can be decribed as a collection of items and attributes.

Items: objects/entities you want to visualize
Attributes: properties of these objects/entities
```

-	First step in data abstraction is to distinguish between two broad classes of dataset types.
-	First class is tables and second class is networks and trees.

---

-	데이터세트는 항목과 그 속성의 모음으로 설명될 수 있다.
-	아이템은 시각화하려는 대상(객체)이고, 속성은 대상의 특성을 말한다.  
-	데이터세트 형태는 크게 두 가지로 나눌 수 있는데, 데이터 추상의 첫 번째 단계는 이 둘을 구별하는 것이다.
-	데이터세트 형태는 테이블과 네트워크 또는 트리가 있다.  

*[img2] tables of dataset types* ![image of tables](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/tables.png)

-	Tables is a grid or collection of columns and rows where every row in the table represents one item, one object of the dataset and every column represents one attribute of these objects.
-	So, an attribute is a characteristic for this object.

---

-	테이블은 행과 열로 구성되어 있고, 행은 항목 또는 객체를 나타내고 열은 속성을 나타낸다.
-	각 각의 항목은 같은 수의 속성과 같은 유형의 속성을 가지고 있어야 한다.

*[img3] networks and trees of dataset types* ![image of networks](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/networks.png)

-	Networks and trees is an idea that the defining characteristic of these collection of itmes is that there are linked together by links.
-	This have nodes(items) and links that connect nodes.
-	Nodes and links can have atrributes associated to thme.
-	Attributes describe characteristic of nodes and links.

---

-	네트워크 또는 트리는 항목이 링크로 연결되어있는 특징을 가지고 있다.
-	즉, 네트워크는 노드(항목)와 노드와 연결되어 있는 링크로 구성되며, 이들도 특성을 가질 수 있다.
-	특성은 노드와 링크의 특징을 설명하며, 예를 들어 노드의 사이즈 등을 결정한다.

### Attribute Types

#### #. day 02, 190102

There are three main types of attributes

-	Categorical - Two or more categories but no intrinsic order

	-	simple ex) gender: male, female
	-	product sales data set ex) product: office supplies, technology, furniture

-	Ordinal

	-	The categories have an order
	-	but, it is not meaningful to perform any arithmetic operation between these categories
	-	simple ex) economic status: low, medium, high
	-	product sales data set ex) order priority: low, medium, high, critical

-	Quantitative

	-	The values represent a measured qunatity
	-	in general, with quantitative attributes, you can perform any kind of arithmetic operation among them
	-	simple ex) weight: 60kg, 81kg, 94kg...
	-	product sales data set ex) sales: 261.54, 10123.02, 244.57...

---

-	속성은 세가지 유형으로 구분될 수 있다.
-	범주형 자료는 두 개 이상의 범주로 구성되며, 이 들 사이의 순서는 의미가 없다.
-	순위형 자료는 두 개 이상의 범주를 가지며, 이 들 사이의 순서가 존재한다. 단, 순서 사이의 거리를 알 수 없기 때문에 산수적 계산은 의미가 없다.
-	양적 자료의 값은 측정된 수량으로 표현되기 때문에, 이들 사이의 산수적 계산이 가능하다.  

### Attribute Semantics(Characteristic)

#### #. day 03, 190103

-	Spatial and Temporal Semantics: Attribue that have spatial or temporal meaning
	-	ex) Spatial: Region(categorial), Latitude & Longitude(quantitative)
	-	ex) Temporal : Order date(quantitative)
-	Sequential, Diverging and Cyclic
	-	ex) Diverging: Profit(quantitative having zero value)
	-	ex) Cyclic: Month of order date(quantitative)
-	Hierarchical
	-	ex) Product category(categorical) > Product sub-category(categorical)

---

-	사전에 정의된 속성의 의미(또는 특징)는 여러가지가 있다.
-	Spatial은 공간의 의미, Temporal은 시간의 의미를 가진다.
-	Sequential은 한쪽 방향의 의미만 가지지만, Diverging은 양쪽 방향의 의미를 가지고 있어 0을 중심으로 음수, 양수를 모두 포함한다.
-	Cyclic은 년, 월, 요일과 같은 주기성을 의미하고, Hierarchical은 하위 항목을 가지는 위계적인 구조를 의미한다.
-	주로 시간과 주기를 나타내는 자료는 양적 자료와 관련이 있다.

### Example for Attribute Types and Semantics

#### #. day 04, 190104

-	`Categorical` Coustomer segment: consumer, corporate, home office, small business
-	`Categorical`,`Spatial`,`Hierarchical` Region: Atlantic, Nunavut, ontario..., Province: New Brimswick, Nova Scotia, Nunavut...
-	`Ordinal` or `Categorical` Order ID: 16326, 8710, 50657...
-	`Ordinal` or `Categorical` Product Container: jumbo box, jumbo drum, large box, medium box, small box...

---

-	속성의 유형이나 의미는 데이터에 대한 이해 정도에 따라 다르게 나타날 수 있다.
-	위의 세 번째 예시에서 Order ID의 숫자가 양적 자료가 아니고, 순서를 가지고 있는 순위형 자료라는 것을 알기 위해서는 데이터에 대한 사전 이해가 필요하다.

### Data Abstraction to Visualization

#### #. day 06, 190106

knowing what kind of attribute and attribute meaning will give you guidance in selecting appropriate visual representations.

*[img4] Line chart* ![Image of Line chart](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/linechart.png)

-	In the first chart, I have the x-axis of the time and the y-axis of the quantity change over time.
-	This is appropriate use of the line chart.
-	Line chart on the right side tries to use exactly the same design, but on the x-axis, I have a number of categories.
-	When you look at this chart, you might think that what this chart shows is changing over time.
-	But in fact there is no particular trend and patterns are not meaningful here.

---

-	왼쪽의 차트는 x축이 시간, y축은 시간에 따라 변하는 양을 보여준다.
-	이러한 데이터는 선차트를 사용하는 것이 적절하다.
-	오른쪽 차트는 x축이 범주형으로 구성되어 있다. 왼쪽과 완전히 동일한 선차트이기 때문에 우리는 시간에 따라 변한다고 생각할 수 있다.  
-	그러나, x축이 범주형이기 때문에 차트의 선은 추세를 나타내는 것이 아니며, 여기서 선의 패턴은 의미가 없다.  

*[img5] Bar chart* ![Image of bar  chart](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/barchart.png)

-	Bar charts can accommodate information about categories, frequencies, or statistics associated with these categories.
-	Here, I reorder this bar chart according to the values, frequencies, or statistics that is map to the height of the bar.
-	Often, being able to reorder bar chart is very useful because it allows us to more reasily read the progression of values.

---

-	막대차트에는 범주형 자료와, 빈도와 같이 범주형 자료에 관련된 통계를 적용시킬 수 있다.
-	오른쪽 차트는 막대의 높이에 매핑되는 값, 빈도 또는 통계에 따라서 막대 차트 순서를 변경한 것이다.
-	오른쪽 차트에서 값의 진행 과정을 보다 쉽게 읽을 수 있기 때문에 막대 차트의 순서를 바꾸는 것은 매우 유용하다.

*[img6] Map* ![Image of map](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/spatial.png)

-	What we know is that if we possess spatial information, spatial attributes, we know that using a spatial representation like a map is one of the options available.
-	But, using a map is not necessarily the best solution always when we like to visualize spatial data.

---

-	공간에 관련된 속성을 가지고 있다면 지도와 같은 공간 표현은 가능한 옵션 중 하나이다.
-	그러나 지도를 사용하는 것이 공간 데이터를 시각화 할 때 항상 최선의 해결책은 아니다.

*[img7] Heat map or Matrix* ![Image of heat map](https://github.com/deepnsoul/TIL/blob/master/foundations/fig/diverging.png)

-	We have a heat map also called matrix, when we have two categorial attributes and at the intersection of these two category attributes, we have a quantity that is actually diverging, it is a diverging quantitative attributes.
-	In the first above, display the value of this quantitative attribute through a color scale that uses different levels of color tone.
-	While in the other below, we have three main colors used, three kinds of main colors. We have red, white, and blue
-	Zero value is map to white, and positive values ​​are map to different color intensities of blue, and negative values ​​are map to different color intensities of red.
-	First above, it is difficult to distinguish between positive and negative, while the second is very easy to distinguish between negative and positive values.
-	Again, knowing characteristics of the attribute helps us make specific decisions about how to visualize this attribute.

---

-	두 개의 범주형 속성이 있고, 이 두 범주형 속성의 교차 부분에 발산하는 양이있을 때 히트 맵 또는 매트릭스를 사용할 수 있다. 이것을 발산하는 양적 속성이라고 부른다.
-	왼쪽 히트 맵에서는 양적 속성의 값을 한 색상 계열의 여러가지 톤을 이용하여 표시하였다.
-	오른쪽 히트 맵에서는 빨간색, 흰색, 파란색의 3 가지 주요 색상을 사용하였다.
-	0 값은 흰색으로 매핑되고 양수 값은 파란색 색상 계열의 강도에 따라 다른 톤으로 매핑하였고 음수 값은 빨간색 계열의 색상으로 매핑하였다.
-	오른쪽 히트 맵은 음수 양수를 구별하기가 어려운 반면, 오른쪽은 그것을 구별하기가 쉽다.
-	속성의 특징을 아는 것은 시각화하는 방법에 대한 구체적인 결정을 내리는데 도움을 준다.

### Data Profiling

#### #. day 07, 190107

You have to become familiar with your data set to connect data abstraction.

-	`Data familiarization and profiling`
	-	Data coming from different sources
	-	Meaning of data often not evident
	-	Effort and interactions needed to understand meaning

---

-	데이터 추상을 진행하기에 앞서 현재 가지고 있는 데이터 세트에 친숙해지는 과정, 데이터 프로파일링이 필요하다.
-	여러 다른 출처로부터 데이터가 수집되고, 종종 그 의미가 불분명하기도 하다.
-	따라서, 데이터를 제공하는 클라이언트와의 커뮤니케이션 노력을 통해 데이터의 각 속성의 의미에 대해 훨씬 더 깊은 이해가 선행되어야 한다.  

Another very important activity usually perform at the beginning of the data visualization project is checking data quality and doing what we call data wrangling.

-	`Data Quality and "wrangling"`
	-	Data quality means that data often comes in ways that are not necessarily precise or complete.
	-	ex) missing values, wrong values
	-	The activities necessary to identify and fix these problems so that you can change this sum of values ​​for your data or even transfer your data from one type to another.

---

-	또한 일반적으로 데이터 시각화 전에 선행되어야 할 중요한 작업은 데이터 품질을 확인하는 데이터 wrangling이다.
-	데이터 품질을 확인하는 것이 중요한 이유는 데이터가 종종 정확하지 않거나 완전하지 않게 제공되기 때문이다.
-	예를 들면 누락된 값이나, 측정 및 입력 이상으로 인한 잘못된 값이 데이터 세트에 포함될 수 있다.
-	따라서 이러한 문제점을 해결하기 위해 데이터 총 개수를 수정하거나 데이터의 유형을 다르게 변경할 수 있다.
-	이 과정의 자세한 부분은 이번 코스에서는 다루지 않는다.
