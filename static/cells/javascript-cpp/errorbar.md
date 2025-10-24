##ErrorBar
Represents error bar of data series.
## ErrorBar class
Represents error bar of data series.
```javascript
class ErrorBar extends Line;
```
### Example
```javascript
const { Workbook, ChartType, ErrorBarDisplayType, ErrorBarType } = AsposeCells;
var workbook = new Workbook();
var cells = workbook.worksheets.get(0).cells;
cells.get("a1").putValue(2);
cells.get("a2").putValue(5);
cells.get("a3").putValue(3);
cells.get("a4").putValue(6);
cells.get("b1").putValue(4);
cells.get("b2").putValue(3);
cells.get("b3").putValue(6);
cells.get("b4").putValue(7);
cells.get("C1").putValue("Q1");
cells.get("C2").putValue("Q2");
cells.get("C3").putValue("Y1");
cells.get("C4").putValue("Y2");
var chartIndex = workbook.worksheets.get(0).charts.add(ChartType.Column, 11, 0, 27, 10);
var chart = workbook.worksheets.get(0).charts.get(chartIndex);
chart.nSeries.add("A1:B4", true);
chart.nSeries.categoryData = "C1:C4";
for (var i = 0; i < chart.nSeries.count; i++) {
var aseries = chart.nSeries.get(i);
aseries.xErrorBar.displayType = ErrorBarDisplayType.Minus;
aseries.xErrorBar.type = ErrorBarType.FixedValue;
aseries.xErrorBar.amount = 5;
}
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Line)](#constructor-line-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| ErrorBarType | Represents error bar amount type. |
| [displayType](#displayType--)| ErrorBarDisplayType | Represents the display type of error bar. |
| [amount](#amount--)| number | Represents amount of error bar. |
| [showMarkerTTop](#showMarkerTTop--)| boolean | Indicates if formatting error bars with a T-top. |
| [plusValue](#plusValue--)| string | Represents positive error amount when error bar type is Custom. |
| [minusValue](#minusValue--)| string | Represents negative error amount when error bar type is Custom. |
| [compoundType](#compoundType--)| MsoLineStyle | Specifies the compound line type |
| [dashType](#dashType--)| MsoLineDashStyle | Specifies the dash line type |
| [capType](#capType--)| LineCapType | Specifies the ending caps. |
| [joinType](#joinType--)| LineJoinType | Specifies the joining caps. |
| [beginType](#beginType--)| MsoArrowheadStyle | Specifies an arrowhead for the begin of a line. |
| [endType](#endType--)| MsoArrowheadStyle | Specifies an arrowhead for the end of a line. |
| [beginArrowLength](#beginArrowLength--)| MsoArrowheadLength | Specifies the length of the arrowhead for the begin of a line. |
| [endArrowLength](#endArrowLength--)| MsoArrowheadLength | Specifies the length of the arrowhead for the end of a line. |
| [beginArrowWidth](#beginArrowWidth--)| MsoArrowheadWidth | Specifies the width of the arrowhead for the begin of a line. |
| [endArrowWidth](#endArrowWidth--)| MsoArrowheadWidth | Specifies the width of the arrowhead for the end of a line. |
| [themeColor](#themeColor--)| ThemeColor | Gets and sets the theme color. |
| [color](#color--)| Color | Represents the [Color](../color/) of the line. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [style](#style--)| LineType | Represents the style of the line. |
| [weight](#weight--)| WeightType | Gets or sets the [WeightType](../weighttype/) of the line. |
| [weightPt](#weightPt--)| number | Gets or sets the weight of the line in unit of points. |
| [weightPx](#weightPx--)| number | Gets or sets the weight of the line in unit of pixels. |
| [formattingType](#formattingType--)| ChartLineFormattingType | Gets or sets format type. |
| [isAutomaticColor](#isAutomaticColor--)| boolean | Readonly. Indicates whether the color of line is automatic assigned. |
| [isVisible](#isVisible--)| boolean | Represents whether the line is visible. |
| [isAuto](#isAuto--)| boolean | Indicates whether this line style is auto assigned. |
| [gradientFill](#gradientFill--)| GradientFill | Readonly. Represents gradient fill. |
### constructor(Line) {#constructor-line-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Line);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Line | The parent object. |
### type {#type--}
Represents error bar amount type.
```javascript
type : ErrorBarType;
```
**Example**
```javascript
const { Workbook, ChartType, ErrorBarType } = AsposeCells;
var workbook = new Workbook();
var cells = workbook.worksheets.get(0).cells;
cells.get("a1").putValue(2);
cells.get("a2").putValue(5);
cells.get("a3").putValue(3);
cells.get("a4").putValue(6);
cells.get("b1").putValue(4);
cells.get("b2").putValue(3);
cells.get("b3").putValue(6);
cells.get("b4").putValue(7);
cells.get("C1").putValue("Q1");
cells.get("C2").putValue("Q2");
cells.get("C3").putValue("Y1");
cells.get("C4").putValue("Y2");
var chartIndex = workbook.worksheets.get(0).charts.add(ChartType.Column, 11, 0, 27, 10);
var chart = workbook.worksheets.get(0).charts.get(chartIndex);
chart.nSeries.add("A1:B4", true);
chart.nSeries.categoryData = "C1:C4";
for (var i = 0; i < chart.nSeries.count; i++) {
var aseries = chart.nSeries.get(i);
//Sets custom error bar type
aseries.xErrorBar.type = ErrorBarType.Custom;
aseries.xErrorBar.plusValue = "=Sheet1!A1";
aseries.xErrorBar.minusValue = "=Sheet1!A2";
}
```
### displayType {#displayType--}
Represents the display type of error bar.
```javascript
displayType : ErrorBarDisplayType;
```
### amount {#amount--}
Represents amount of error bar.
```javascript
amount : number;
```
**Remarks**
The amount must be greater than or equal to zero.
### showMarkerTTop {#showMarkerTTop--}
Indicates if formatting error bars with a T-top.
```javascript
showMarkerTTop : boolean;
```
### plusValue {#plusValue--}
Represents positive error amount when error bar type is Custom.
```javascript
plusValue : string;
```
### minusValue {#minusValue--}
Represents negative error amount when error bar type is Custom.
```javascript
minusValue : string;
```
### compoundType {#compoundType--}
Specifies the compound line type
```javascript
compoundType : MsoLineStyle;
```
### dashType {#dashType--}
Specifies the dash line type
```javascript
dashType : MsoLineDashStyle;
```
### capType {#capType--}
Specifies the ending caps.
```javascript
capType : LineCapType;
```
### joinType {#joinType--}
Specifies the joining caps.
```javascript
joinType : LineJoinType;
```
### beginType {#beginType--}
Specifies an arrowhead for the begin of a line.
```javascript
beginType : MsoArrowheadStyle;
```
### endType {#endType--}
Specifies an arrowhead for the end of a line.
```javascript
endType : MsoArrowheadStyle;
```
### beginArrowLength {#beginArrowLength--}
Specifies the length of the arrowhead for the begin of a line.
```javascript
beginArrowLength : MsoArrowheadLength;
```
### endArrowLength {#endArrowLength--}
Specifies the length of the arrowhead for the end of a line.
```javascript
endArrowLength : MsoArrowheadLength;
```
### beginArrowWidth {#beginArrowWidth--}
Specifies the width of the arrowhead for the begin of a line.
```javascript
beginArrowWidth : MsoArrowheadWidth;
```
### endArrowWidth {#endArrowWidth--}
Specifies the width of the arrowhead for the end of a line.
```javascript
endArrowWidth : MsoArrowheadWidth;
```
### themeColor {#themeColor--}
Gets and sets the theme color.
```javascript
themeColor : ThemeColor;
```
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
### color {#color--}
Represents the [Color](../color/) of the line.
```javascript
color : Color;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### style {#style--}
Represents the style of the line.
```javascript
style : LineType;
```
### weight {#weight--}
Gets or sets the [WeightType](../weighttype/) of the line.
```javascript
weight : WeightType;
```
### weightPt {#weightPt--}
Gets or sets the weight of the line in unit of points.
```javascript
weightPt : number;
```
### weightPx {#weightPx--}
Gets or sets the weight of the line in unit of pixels.
```javascript
weightPx : number;
```
### formattingType {#formattingType--}
Gets or sets format type.
```javascript
formattingType : ChartLineFormattingType;
```
### isAutomaticColor {#isAutomaticColor--}
Readonly. Indicates whether the color of line is automatic assigned.
```javascript
isAutomaticColor : boolean;
```
### isVisible {#isVisible--}
Represents whether the line is visible.
```javascript
isVisible : boolean;
```
### isAuto {#isAuto--}
Indicates whether this line style is auto assigned.
```javascript
isAuto : boolean;
```
### gradientFill {#gradientFill--}
Readonly. Represents gradient fill.
```javascript
gradientFill : GradientFill;
```
