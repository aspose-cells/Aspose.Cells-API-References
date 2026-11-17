---
title: "Clase ChartPoint"
linktitle: "ChartPoint"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase ChartPoint. Encapsula el objeto que representa chartpoint en Go."
type: docs
weight: 200
url: /es/go-cpp/chartpoint/
---

## ChartPoint class

Represents a single point in a series in a chart.

```go

type ChartPoint struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetExplosion](./getexplosion/) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [SetExplosion](./setexplosion/) | La distancia de una porción de pastel abierta desde el centro del gráfico de pastel se expresa como un porcentaje del diámetro del pastel. |
| [GetShadow](./getshadow/) | Verdadero si el chartpoint tiene una sombra. |
| [SetShadow](./setshadow/) | Verdadero si el chartpoint tiene una sombra. |
| [GetBorder](./getborder/) | Gets the Line</see>. |
| [GetArea](./getarea/) | Gets the Area</see>. |
| [GetMarker](./getmarker/) | Obtiene el Marker</see>. |
| [GetDataLabels](./getdatalabels/) | Devuelve un objeto DataLabels que representa la etiqueta de datos asociada a este punto de gráfico. |
| [Get_YValue](./get_yvalue/) | Obtiene o establece el valor Y del punto del gráfico. |
| [SetYValue](./setyvalue/) | Obtiene o establece el valor Y del punto del gráfico. |
| [GetYValueType](./getyvaluetype/) | Obtiene el tipo de valor Y del punto del gráfico. |
| [GetXValue](./getxvalue/) | Obtiene o establece el valor X del punto del gráfico. |
| [SetXValue](./setxvalue/) | Obtiene o establece el valor X del punto del gráfico. |
| [GetXValueType](./getxvaluetype/) | Obtiene el tipo de valor X del punto del gráfico. |
| [GetShapeProperties](./getshapeproperties/) | Obtiene el objeto ShapePropertyCollection que contiene las propiedades visuales de forma del ChartPoint. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | Obtiene o establece un valor que indica si este punto de datos está en el segundo sector o barra de un gráfico de pastel o barra de pastel. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | Obtiene o establece un valor que indica si este punto de datos está en el segundo sector o barra de un gráfico de pastel o barra de pastel. |
| [GetShapeX](./getshapex/) | Obtiene la coordenada x de la esquina superior izquierda en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate(). |
| [GetShapeY](./getshapey/) | Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate(). |
| [GetShapeWidth](./getshapewidth/) | Obtiene el ancho en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate(). |
| [GetShapeHeight](./getshapeheight/) | Obtiene la altura en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate(). |
| [GetShapeXPx](./getshapexpx/) | Obtiene la coordenada x de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [GetShapeYPx](./getshapeypx/) | Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [GetShapeWidthPx](./getshapewidthpx/) | Obtiene el ancho en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [GetShapeHeightPx](./getshapeheightpx/) | Obtiene la altura en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [GetBorderWidthPx](./getborderwidthpx/) | Obtiene el ancho del borde en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [GetRadiusPx](./getradiuspx/) | Obtiene el radio de burbuja, pastel o Doughnut en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Obtiene el radio interno de la porción de Doughnut en unidades de píxeles después de llamar al método Chart.Calculate(). Aplica al gráfico Doughnut. |
| [GetStartAngle](./getstartangle/) | Obtiene el ángulo inicial para la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). Aplica al gráfico Pie. |
| [GetEndAngle](./getendangle/) | Obtiene el ángulo final para la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). Aplica al gráfico Pie. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | Obtiene la coordenada x del punto inicial para la sección de pastel después de llamar al método Chart.Calculate(). Aplica a los gráficos Pie y Doughnut. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | Obtiene la coordenada y del punto inicial para la sección de pastel después de llamar al método Chart.Calculate(). Aplica a los gráficos Pie y Doughnut. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | Obtiene la coordenada x del punto final para la sección de pastel después de llamar al método Chart.Calculate(). Aplica a los gráficos Pie y Doughnut. |
| [GetArcEndPointYPx](./getarcendpointypx/) | Obtiene la coordenada y del punto final para la sección de pastel después de llamar al método Chart.Calculate(). Aplica a los gráficos Pie y Doughnut. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Obtiene la coordenada x del punto inicial para la sección de pastel después de llamar al método Chart.Calculate(). Aplica al gráfico Doughnut. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Obtiene la coordenada y del punto inicial para la sección de pastel después de llamar al método Chart.Calculate(). Aplica al gráfico Doughnut. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate().Aplica a los gráficos de dona. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Obtiene la coordenada y del punto final de la sección de pastel después de llamar al método Chart.Calculate().Aplica al gráfico de dona. |
| [GetTopPointCount](./gettoppointcount/) | Obtiene el número de puntos superiores después de llamar al método Chart.Calculate(). |
| [GetTopPointXPx](./gettoppointxpx/) | Obtiene la coordenada x del punto superior de la forma después de llamar al método Chart.Calculate().Aplica a gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid y Area3D |
| [GetTopPointYPx](./gettoppointypx/) | Obtiene la coordenada y del punto superior de la forma después de llamar al método Chart.Calculate().Aplica a gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid y Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | Obtiene el número de puntos inferiores después de llamar al método Chart.Calculate(). |
| [GetBottomPointXPx](./getbottompointxpx/) | Obtiene la coordenada x del punto inferior de la forma después de llamar al método Chart.Calculate().Aplica a gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetBottomPointYPx](./getbottompointypx/) | Obtiene la coordenada y del punto inferior de la forma después de llamar al método Chart.Calculate().Aplica a gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Obtiene el número de puntos en el eje de categorías después de llamar al método Chart.Calculate().Solo se aplica a los gráficos de área. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Obtiene la coordenada x del punto en el eje de categorías después de llamar al método Chart.Calculate().Solo se aplica al gráfico de área. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Obtiene la coordenada y del punto en el eje de categorías después de llamar al método Chart.Calculate().Solo se aplica al gráfico de área. |
