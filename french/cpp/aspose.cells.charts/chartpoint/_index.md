---
title: Aspose::Cells::Charts::ChartPoint class
linktitle: ChartPoint
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartPoint class. Represents a single point in a series in a chart in C++.'
type: docs
weight: 1000
url: /fr/cpp/aspose.cells.charts/chartpoint/
---
## ChartPoint class


Represents a single point in a series in a chart.

```cpp
class ChartPoint
```

## Methods

| Method | Description |
| --- | --- |
| [ChartPoint(ChartPoint_Impl* impl)](./chartpoint/) | Constructs from an implementation object. |
| [ChartPoint(const ChartPoint\& src)](./chartpoint/) | Copy constructor. |
| [Get_YValue()](./get_yvalue/) | Gets or sets the Y value of the chart point. |
| [GetArcEndPointXPx()](./getarcendpointxpx/) | Gets the x coordinate of ending point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Pie and Doughnut chart. |
| [GetArcEndPointYPx()](./getarcendpointypx/) | Gets the y coordinate of ending point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Pie and Doughnut chart. |
| [GetArcStartPointXPx()](./getarcstartpointxpx/) | Gets the x coordinate of starting point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Pie and Doughnut chart. |
| [GetArcStartPointYPx()](./getarcstartpointypx/) | Gets the y coordinate of starting point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Pie and Doughnut chart. |
| [GetArea()](./getarea/) | Gets the [area](../). |
| [GetBorder()](./getborder/) | Gets the [border](../). |
| [GetBorderWidthPx()](./getborderwidthpx/) | Gets the width of border in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetBottomPointCount()](./getbottompointcount/) | Gets the number of bottom points after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetBottomPointXPx(int32_t index)](./getbottompointxpx/) | Gets x-coordinate of the bottom point of shape after calls [Chart.Calculate()](../chart/calculate/) method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetBottomPointYPx(int32_t index)](./getbottompointypx/) | Gets y-coordinate of the bottom point of shape after calls [Chart.Calculate()](../chart/calculate/) method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetDataLabels()](./getdatalabels/) | Returns a [DataLabels](../datalabels/) object that represents the data label associated with this chart point. |
| [GetDoughnutInnerRadius()](./getdoughnutinnerradius/) | Gets the inner radius of doughnut slice in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Doughnut chart. |
| [GetEndAngle()](./getendangle/) | Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Pie chart. |
| [GetExplosion()](./getexplosion/) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [GetInnerArcEndPointXPx()](./getinnerarcendpointxpx/) | Gets the x coordinate of ending point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Doughnut chart. |
| [GetInnerArcEndPointYPx()](./getinnerarcendpointypx/) | Gets the y coordinate of ending point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Doughnut chart. |
| [GetInnerArcStartPointXPx()](./getinnerarcstartpointxpx/) | Gets the x coordinate of starting point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Doughnut chart. |
| [GetInnerArcStartPointYPx()](./getinnerarcstartpointypx/) | Gets the y coordinate of starting point for the pie section after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Doughnut chart. |
| [GetInnerRadiusPx()](./getinnerradiuspx/) |  **(Deprecated)** Gets the inner radius of doughnut slice in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Doughnut chart. |
| [GetMarker()](./getmarker/) | Gets the [marker](../marker/). |
| [GetOnCategoryAxisPointCount()](./getoncategoryaxispointcount/) | Gets the number of the points on category axis after calls [Chart.Calculate()](../chart/calculate/) method. Only applies to area chart. |
| [GetOnCategoryAxisPointXPx(int32_t index)](./getoncategoryaxispointxpx/) | Gets x-coordinate of the point on category axis after calls [Chart.Calculate()](../chart/calculate/) method. Only applies to Area chart. |
| [GetOnCategoryAxisPointYPx(int32_t index)](./getoncategoryaxispointypx/) | Gets y-coordinate of the point on category axis after calls [Chart.Calculate()](../chart/calculate/) method. Only applies to Area chart. |
| [GetRadiusPx()](./getradiuspx/) | Gets the radius of bubble, pie or doughnut in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShadow()](./getshadow/) | True if the chartpoint has a shadow. |
| [GetShapeHeight()](./getshapeheight/) | Gets the height in units of 1/4000 of chart's height after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShapeHeightPx()](./getshapeheightpx/) | Gets the height in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShapeProperties()](./getshapeproperties/) | Gets the ShapePropertyCollection object that holds the visual shape properties of the [ChartPoint](./). |
| [GetShapeWidth()](./getshapewidth/) | Gets the width in units of 1/4000 of chart's width after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShapeWidthPx()](./getshapewidthpx/) | Gets the width in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShapeX()](./getshapex/) | Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShapeXPx()](./getshapexpx/) | Gets the x coordinate of the upper left corner in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShapeY()](./getshapey/) | Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetShapeYPx()](./getshapeypx/) | Gets the y coordinate of the upper left corner in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetStartAngle()](./getstartangle/) | Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls [Chart.Calculate()](../chart/calculate/) method. Applies to Pie chart. |
| [GetTopPointCount()](./gettoppointcount/) | Gets the number of top points after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetTopPointXPx(int32_t index)](./gettoppointxpx/) | Gets x-coordinate of the top point of shape after calls [Chart.Calculate()](../chart/calculate/) method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D. |
| [GetTopPointYPx(int32_t index)](./gettoppointypx/) | Gets y-coordinate of the top point of shape after calls [Chart.Calculate()](../chart/calculate/) method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D. |
| [GetXValue()](./getxvalue/) | Gets or sets the X value of the chart point. |
| [GetXValueType()](./getxvaluetype/) | Gets X value type of the chart point. |
| [GetYValueType()](./getyvaluetype/) | Gets Y value type of the chart point. |
| [IsInSecondaryPlot()](./isinsecondaryplot/) | Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartPoint\& src)](./operator_asm/) | operator= |
| [SetExplosion(int32_t value)](./setexplosion/) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [SetIsInSecondaryPlot(bool value)](./setisinsecondaryplot/) | Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart. |
| [SetShadow(bool value)](./setshadow/) | True if the chartpoint has a shadow. |
| [SetXValue(const Aspose::Cells::Object\& value)](./setxvalue/) | Gets or sets the X value of the chart point. |
| [SetYValue(const Aspose::Cells::Object\& value)](./setyvalue/) | Gets or sets the Y value of the chart point. |
| [~ChartPoint()](./~chartpoint/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instanciation d'un objet Workbook
Workbook workbook;

//Obtention de la référence de la première feuille de calcul
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Ajouter une valeur d'exemple à la cellule \"A1\"
worksheet.GetCells().Get(u"A1").PutValue(50);

//Ajouter une valeur d'exemple à la cellule \"A2\"
worksheet.GetCells().Get(u"A2").PutValue(100);

//Ajouter une valeur d'exemple à la cellule \"A3\"
worksheet.GetCells().Get(u"A3").PutValue(150);

//Ajouter une valeur d'exemple à la cellule \"B1\"
worksheet.GetCells().Get(u"B1").PutValue(60);

//Ajouter une valeur d'exemple à la cellule \"B2\"
worksheet.GetCells().Get(u"B2").PutValue(32);

//Ajouter une valeur d'exemple à la cellule \"B3\"
worksheet.GetCells().Get(u"B3").PutValue(50);

//Ajouter un graphique à la feuille de calcul
int chartIndex = worksheet.GetCharts().Add(ChartType::PieExploded, 5, 0, 25, 10);

//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.GetCharts().Get(chartIndex);

//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
chart.GetNSeries().Add(u"A1:B3", true);

//Afficher les étiquettes de données
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

for (int i = 0; i < chart.GetNSeries().Get(0).GetPoints().GetCount(); i++)
{
    //Obtenir le point de données
    ChartPoint point = chart.GetNSeries().Get(0).GetPoints().Get(i);
    //Définir l'explosion Pir
    point.SetExplosion(15);
    //Définir la couleur de bordure
    point.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
}

//Enregistrement du fichier Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
