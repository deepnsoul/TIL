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
