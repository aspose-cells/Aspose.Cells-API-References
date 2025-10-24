##ChartPoint Class
'ChartPoint class. Encapsulates the object that represents chartpoint in Go.'
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
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetExplosion](./getexplosion/) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
|[SetExplosion](./setexplosion/) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
|[GetShadow](./getshadow/) | True if the chartpoint has a shadow. |
|[SetShadow](./setshadow/) | True if the chartpoint has a shadow. |
|[GetBorder](./getborder/) | Gets the Line</see>. |
|[GetArea](./getarea/) | Gets the Area</see>. |
|[GetMarker](./getmarker/) | Gets the Marker</see>. |
|[GetDataLabels](./getdatalabels/) | Returns a DataLabels object that represents the data label associated with this chart point. |
|[Get_YValue](./get_yvalue/) | Gets or sets the Y value of the chart point. |
|[SetYValue](./setyvalue/) | Gets or sets the Y value of the chart point. |
|[GetYValueType](./getyvaluetype/) | Gets Y value type of the chart point. |
|[GetXValue](./getxvalue/) | Gets or sets the X value of the chart point. |
|[SetXValue](./setxvalue/) | Gets or sets the X value of the chart point. |
|[GetXValueType](./getxvaluetype/) | Gets X value type of the chart point. |
|[GetShapeProperties](./getshapeproperties/) | Gets the ShapePropertyCollection object that holds the visual shape properties of the ChartPoint. |
|[IsInSecondaryPlot](./isinsecondaryplot/) | Gets or sets a value indicates whether this data points is in the second pie or baron a pie of pie or bar of pie chart |
|[SetIsInSecondaryPlot](./setisinsecondaryplot/) | Gets or sets a value indicates whether this data points is in the second pie or baron a pie of pie or bar of pie chart |
|[GetShapeX](./getshapex/) | Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
|[GetShapeY](./getshapey/) | Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
|[GetShapeWidth](./getshapewidth/) | Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
|[GetShapeHeight](./getshapeheight/) | Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
|[GetShapeXPx](./getshapexpx/) | Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
|[GetShapeYPx](./getshapeypx/) | Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
|[GetShapeWidthPx](./getshapewidthpx/) | Gets the width in units of pixels after calls Chart.Calculate() method. |
|[GetShapeHeightPx](./getshapeheightpx/) | Gets the height in units of pixels after calls Chart.Calculate() method. |
|[GetBorderWidthPx](./getborderwidthpx/) | Gets the width of border in units of pixels after calls Chart.Calculate() method. |
|[GetRadiusPx](./getradiuspx/) | Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
|[GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method.Applies to Doughnut chart. |
|[GetStartAngle](./getstartangle/) | Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method.Applies to Pie chart. |
|[GetEndAngle](./getendangle/) | Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method.Applies to Pie chart. |
|[GetArcStartPointXPx](./getarcstartpointxpx/) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method.Applies to Pie and Doughnut  chart. |
|[GetArcStartPointYPx](./getarcstartpointypx/) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method.Applies to Pie and Doughnut  chart. |
|[GetArcEndPointXPx](./getarcendpointxpx/) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method.Applies to Pie and Doughnut  chart. |
|[GetArcEndPointYPx](./getarcendpointypx/) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method.Applies to Pie and Doughnut chart. |
|[GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method.Applies to Doughnut chart. |
|[GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method.Applies to Doughnut chart. |
|[GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method.Applies to Doughnut chart. |
|[GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method.Applies to Doughnut chart. |
|[GetTopPointCount](./gettoppointcount/) | Gets the number of top points after calls Chart.Calculate() method. |
|[GetTopPointXPx](./gettoppointxpx/) | Gets x-coordinate of the top point of shape after calls Chart.Calculate() method.Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |
|[GetTopPointYPx](./gettoppointypx/) | Gets y-coordinate of the top point of shape after calls Chart.Calculate() method.Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |
|[GetBottomPointCount](./getbottompointcount/) | Gets the number of bottom points  after calls Chart.Calculate() method. |
|[GetBottomPointXPx](./getbottompointxpx/) | Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method.Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
|[GetBottomPointYPx](./getbottompointypx/) | Gets y-coordinate of the bottom point of shape  after calls Chart.Calculate() method.Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
|[GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart. |
|[GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
|[GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
