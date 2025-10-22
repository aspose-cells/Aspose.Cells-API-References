##ErrorBar
Represents error bar of data series.
## ErrorBar class
Represents error bar of data series.
```javascript
class ErrorBar extends Line;
```
### Example
```javascript
const { Workbook, ChartType, ErrorBarDisplayType, ErrorBarType } = require("aspose.cells.node");
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
| Constructor | Description |
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
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Represents error bar amount type. |
| [setType(ErrorBarType)](#setType-errorbartype-)| <b>@deprecated.</b> Please use the 'type' property instead. Represents error bar amount type. |
| [getDisplayType()](#getDisplayType--)| <b>@deprecated.</b> Please use the 'displayType' property instead. Represents the display type of error bar. |
| [setDisplayType(ErrorBarDisplayType)](#setDisplayType-errorbardisplaytype-)| <b>@deprecated.</b> Please use the 'displayType' property instead. Represents the display type of error bar. |
| [getAmount()](#getAmount--)| <b>@deprecated.</b> Please use the 'amount' property instead. Represents amount of error bar. |
| [setAmount(number)](#setAmount-number-)| <b>@deprecated.</b> Please use the 'amount' property instead. Represents amount of error bar. |
| [getShowMarkerTTop()](#getShowMarkerTTop--)| <b>@deprecated.</b> Please use the 'showMarkerTTop' property instead. Indicates if formatting error bars with a T-top. |
| [setShowMarkerTTop(boolean)](#setShowMarkerTTop-boolean-)| <b>@deprecated.</b> Please use the 'showMarkerTTop' property instead. Indicates if formatting error bars with a T-top. |
| [getPlusValue()](#getPlusValue--)| <b>@deprecated.</b> Please use the 'plusValue' property instead. Represents positive error amount when error bar type is Custom. |
| [setPlusValue(string)](#setPlusValue-string-)| <b>@deprecated.</b> Please use the 'plusValue' property instead. Represents positive error amount when error bar type is Custom. |
| [getMinusValue()](#getMinusValue--)| <b>@deprecated.</b> Please use the 'minusValue' property instead. Represents negative error amount when error bar type is Custom. |
| [setMinusValue(string)](#setMinusValue-string-)| <b>@deprecated.</b> Please use the 'minusValue' property instead. Represents negative error amount when error bar type is Custom. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getCompoundType()](#getCompoundType--)| <b>@deprecated.</b> Please use the 'compoundType' property instead. Specifies the compound line type |
| [setCompoundType(MsoLineStyle)](#setCompoundType-msolinestyle-)| <b>@deprecated.</b> Please use the 'compoundType' property instead. Specifies the compound line type |
| [getDashType()](#getDashType--)| <b>@deprecated.</b> Please use the 'dashType' property instead. Specifies the dash line type |
| [setDashType(MsoLineDashStyle)](#setDashType-msolinedashstyle-)| <b>@deprecated.</b> Please use the 'dashType' property instead. Specifies the dash line type |
| [getCapType()](#getCapType--)| <b>@deprecated.</b> Please use the 'capType' property instead. Specifies the ending caps. |
| [setCapType(LineCapType)](#setCapType-linecaptype-)| <b>@deprecated.</b> Please use the 'capType' property instead. Specifies the ending caps. |
| [getJoinType()](#getJoinType--)| <b>@deprecated.</b> Please use the 'joinType' property instead. Specifies the joining caps. |
| [setJoinType(LineJoinType)](#setJoinType-linejointype-)| <b>@deprecated.</b> Please use the 'joinType' property instead. Specifies the joining caps. |
| [getBeginType()](#getBeginType--)| <b>@deprecated.</b> Please use the 'beginType' property instead. Specifies an arrowhead for the begin of a line. |
| [setBeginType(MsoArrowheadStyle)](#setBeginType-msoarrowheadstyle-)| <b>@deprecated.</b> Please use the 'beginType' property instead. Specifies an arrowhead for the begin of a line. |
| [getEndType()](#getEndType--)| <b>@deprecated.</b> Please use the 'endType' property instead. Specifies an arrowhead for the end of a line. |
| [setEndType(MsoArrowheadStyle)](#setEndType-msoarrowheadstyle-)| <b>@deprecated.</b> Please use the 'endType' property instead. Specifies an arrowhead for the end of a line. |
| [getBeginArrowLength()](#getBeginArrowLength--)| <b>@deprecated.</b> Please use the 'beginArrowLength' property instead. Specifies the length of the arrowhead for the begin of a line. |
| [setBeginArrowLength(MsoArrowheadLength)](#setBeginArrowLength-msoarrowheadlength-)| <b>@deprecated.</b> Please use the 'beginArrowLength' property instead. Specifies the length of the arrowhead for the begin of a line. |
| [getEndArrowLength()](#getEndArrowLength--)| <b>@deprecated.</b> Please use the 'endArrowLength' property instead. Specifies the length of the arrowhead for the end of a line. |
| [setEndArrowLength(MsoArrowheadLength)](#setEndArrowLength-msoarrowheadlength-)| <b>@deprecated.</b> Please use the 'endArrowLength' property instead. Specifies the length of the arrowhead for the end of a line. |
| [getBeginArrowWidth()](#getBeginArrowWidth--)| <b>@deprecated.</b> Please use the 'beginArrowWidth' property instead. Specifies the width of the arrowhead for the begin of a line. |
| [setBeginArrowWidth(MsoArrowheadWidth)](#setBeginArrowWidth-msoarrowheadwidth-)| <b>@deprecated.</b> Please use the 'beginArrowWidth' property instead. Specifies the width of the arrowhead for the begin of a line. |
| [getEndArrowWidth()](#getEndArrowWidth--)| <b>@deprecated.</b> Please use the 'endArrowWidth' property instead. Specifies the width of the arrowhead for the end of a line. |
| [setEndArrowWidth(MsoArrowheadWidth)](#setEndArrowWidth-msoarrowheadwidth-)| <b>@deprecated.</b> Please use the 'endArrowWidth' property instead. Specifies the width of the arrowhead for the end of a line. |
| [getThemeColor()](#getThemeColor--)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Represents the [Color](../color/) of the line. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Represents the [Color](../color/) of the line. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getStyle()](#getStyle--)| <b>@deprecated.</b> Please use the 'style' property instead. Represents the style of the line. |
| [setStyle(LineType)](#setStyle-linetype-)| <b>@deprecated.</b> Please use the 'style' property instead. Represents the style of the line. |
| [getWeight()](#getWeight--)| <b>@deprecated.</b> Please use the 'weight' property instead. Gets or sets the [WeightType](../weighttype/) of the line. |
| [setWeight(WeightType)](#setWeight-weighttype-)| <b>@deprecated.</b> Please use the 'weight' property instead. Gets or sets the [WeightType](../weighttype/) of the line. |
| [getWeightPt()](#getWeightPt--)| <b>@deprecated.</b> Please use the 'weightPt' property instead. Gets or sets the weight of the line in unit of points. |
| [setWeightPt(number)](#setWeightPt-number-)| <b>@deprecated.</b> Please use the 'weightPt' property instead. Gets or sets the weight of the line in unit of points. |
| [getWeightPx()](#getWeightPx--)| <b>@deprecated.</b> Please use the 'weightPx' property instead. Gets or sets the weight of the line in unit of pixels. |
| [setWeightPx(number)](#setWeightPx-number-)| <b>@deprecated.</b> Please use the 'weightPx' property instead. Gets or sets the weight of the line in unit of pixels. |
| [getFormattingType()](#getFormattingType--)| <b>@deprecated.</b> Please use the 'formattingType' property instead. Gets or sets format type. |
| [setFormattingType(ChartLineFormattingType)](#setFormattingType-chartlineformattingtype-)| <b>@deprecated.</b> Please use the 'formattingType' property instead. Gets or sets format type. |
| [isAutomaticColor()](#isAutomaticColor--)| <b>@deprecated.</b> Please use the 'isAutomaticColor' property instead. Indicates whether the color of line is automatic assigned. |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents whether the line is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents whether the line is visible. |
| [isAuto()](#isAuto--)| <b>@deprecated.</b> Please use the 'isAuto' property instead. Indicates whether this line style is auto assigned. |
| [setIsAuto(boolean)](#setIsAuto-boolean-)| <b>@deprecated.</b> Please use the 'isAuto' property instead. Indicates whether this line style is auto assigned. |
| [getGradientFill()](#getGradientFill--)| <b>@deprecated.</b> Please use the 'gradientFill' property instead. Represents gradient fill. |
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
const { Workbook, ChartType, ErrorBarType } = require("aspose.cells.node");
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
### getType() {#getType--}
```javascript
getType() : ErrorBarType;
```
**Returns**
[ErrorBarType](../errorbartype/)
### setType(ErrorBarType) {#setType-errorbartype-}
```javascript
setType(value: ErrorBarType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ErrorBarType](../errorbartype/) | The value to set. |
### getDisplayType() {#getDisplayType--}
```javascript
getDisplayType() : ErrorBarDisplayType;
```
**Returns**
[ErrorBarDisplayType](../errorbardisplaytype/)
### setDisplayType(ErrorBarDisplayType) {#setDisplayType-errorbardisplaytype-}
```javascript
setDisplayType(value: ErrorBarDisplayType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ErrorBarDisplayType](../errorbardisplaytype/) | The value to set. |
### getAmount() {#getAmount--}
```javascript
getAmount() : number;
```
**Remarks**
The amount must be greater than or equal to zero.
### setAmount(number) {#setAmount-number-}
```javascript
setAmount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The amount must be greater than or equal to zero.
### getShowMarkerTTop() {#getShowMarkerTTop--}
```javascript
getShowMarkerTTop() : boolean;
```
### setShowMarkerTTop(boolean) {#setShowMarkerTTop-boolean-}
```javascript
setShowMarkerTTop(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPlusValue() {#getPlusValue--}
```javascript
getPlusValue() : string;
```
### setPlusValue(string) {#setPlusValue-string-}
```javascript
setPlusValue(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getMinusValue() {#getMinusValue--}
```javascript
getMinusValue() : string;
```
### setMinusValue(string) {#setMinusValue-string-}
```javascript
setMinusValue(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getCompoundType() {#getCompoundType--}
```javascript
getCompoundType() : MsoLineStyle;
```
**Returns**
[MsoLineStyle](../msolinestyle/)
### setCompoundType(MsoLineStyle) {#setCompoundType-msolinestyle-}
```javascript
setCompoundType(value: MsoLineStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineStyle](../msolinestyle/) | The value to set. |
### getDashType() {#getDashType--}
```javascript
getDashType() : MsoLineDashStyle;
```
**Returns**
[MsoLineDashStyle](../msolinedashstyle/)
### setDashType(MsoLineDashStyle) {#setDashType-msolinedashstyle-}
```javascript
setDashType(value: MsoLineDashStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineDashStyle](../msolinedashstyle/) | The value to set. |
### getCapType() {#getCapType--}
```javascript
getCapType() : LineCapType;
```
**Returns**
[LineCapType](../linecaptype/)
### setCapType(LineCapType) {#setCapType-linecaptype-}
```javascript
setCapType(value: LineCapType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineCapType](../linecaptype/) | The value to set. |
### getJoinType() {#getJoinType--}
```javascript
getJoinType() : LineJoinType;
```
**Returns**
[LineJoinType](../linejointype/)
### setJoinType(LineJoinType) {#setJoinType-linejointype-}
```javascript
setJoinType(value: LineJoinType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineJoinType](../linejointype/) | The value to set. |
### getBeginType() {#getBeginType--}
```javascript
getBeginType() : MsoArrowheadStyle;
```
**Returns**
[MsoArrowheadStyle](../msoarrowheadstyle/)
### setBeginType(MsoArrowheadStyle) {#setBeginType-msoarrowheadstyle-}
```javascript
setBeginType(value: MsoArrowheadStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |
### getEndType() {#getEndType--}
```javascript
getEndType() : MsoArrowheadStyle;
```
**Returns**
[MsoArrowheadStyle](../msoarrowheadstyle/)
### setEndType(MsoArrowheadStyle) {#setEndType-msoarrowheadstyle-}
```javascript
setEndType(value: MsoArrowheadStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |
### getBeginArrowLength() {#getBeginArrowLength--}
```javascript
getBeginArrowLength() : MsoArrowheadLength;
```
**Returns**
[MsoArrowheadLength](../msoarrowheadlength/)
### setBeginArrowLength(MsoArrowheadLength) {#setBeginArrowLength-msoarrowheadlength-}
```javascript
setBeginArrowLength(value: MsoArrowheadLength) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |
### getEndArrowLength() {#getEndArrowLength--}
```javascript
getEndArrowLength() : MsoArrowheadLength;
```
**Returns**
[MsoArrowheadLength](../msoarrowheadlength/)
### setEndArrowLength(MsoArrowheadLength) {#setEndArrowLength-msoarrowheadlength-}
```javascript
setEndArrowLength(value: MsoArrowheadLength) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |
### getBeginArrowWidth() {#getBeginArrowWidth--}
```javascript
getBeginArrowWidth() : MsoArrowheadWidth;
```
**Returns**
[MsoArrowheadWidth](../msoarrowheadwidth/)
### setBeginArrowWidth(MsoArrowheadWidth) {#setBeginArrowWidth-msoarrowheadwidth-}
```javascript
setBeginArrowWidth(value: MsoArrowheadWidth) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |
### getEndArrowWidth() {#getEndArrowWidth--}
```javascript
getEndArrowWidth() : MsoArrowheadWidth;
```
**Returns**
[MsoArrowheadWidth](../msoarrowheadwidth/)
### setEndArrowWidth(MsoArrowheadWidth) {#setEndArrowWidth-msoarrowheadwidth-}
```javascript
setEndArrowWidth(value: MsoArrowheadWidth) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |
### getThemeColor() {#getThemeColor--}
```javascript
getThemeColor() : ThemeColor;
```
**Returns**
[ThemeColor](../themecolor/)
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}
```javascript
setThemeColor(value: ThemeColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
### getColor() {#getColor--}
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
### setColor(Color) {#setColor-color-}
```javascript
setColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getTransparency() {#getTransparency--}
```javascript
getTransparency() : number;
```
### setTransparency(number) {#setTransparency-number-}
```javascript
setTransparency(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getStyle() {#getStyle--}
```javascript
getStyle() : LineType;
```
**Returns**
[LineType](../linetype/)
### setStyle(LineType) {#setStyle-linetype-}
```javascript
setStyle(value: LineType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineType](../linetype/) | The value to set. |
### getWeight() {#getWeight--}
```javascript
getWeight() : WeightType;
```
**Returns**
[WeightType](../weighttype/)
### setWeight(WeightType) {#setWeight-weighttype-}
```javascript
setWeight(value: WeightType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WeightType](../weighttype/) | The value to set. |
### getWeightPt() {#getWeightPt--}
```javascript
getWeightPt() : number;
```
### setWeightPt(number) {#setWeightPt-number-}
```javascript
setWeightPt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getWeightPx() {#getWeightPx--}
```javascript
getWeightPx() : number;
```
### setWeightPx(number) {#setWeightPx-number-}
```javascript
setWeightPx(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFormattingType() {#getFormattingType--}
```javascript
getFormattingType() : ChartLineFormattingType;
```
**Returns**
[ChartLineFormattingType](../chartlineformattingtype/)
### setFormattingType(ChartLineFormattingType) {#setFormattingType-chartlineformattingtype-}
```javascript
setFormattingType(value: ChartLineFormattingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartLineFormattingType](../chartlineformattingtype/) | The value to set. |
### isAutomaticColor() {#isAutomaticColor--}
```javascript
isAutomaticColor() : boolean;
```
### isVisible() {#isVisible--}
```javascript
isVisible() : boolean;
```
### setIsVisible(boolean) {#setIsVisible-boolean-}
```javascript
setIsVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isAuto() {#isAuto--}
```javascript
isAuto() : boolean;
```
### setIsAuto(boolean) {#setIsAuto-boolean-}
```javascript
setIsAuto(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getGradientFill() {#getGradientFill--}
```javascript
getGradientFill() : GradientFill;
```
**Returns**
[GradientFill](../gradientfill/)
