##Trendline
Represents a trendline in a chart.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```
Represents a trendline in a chart.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a sample value to "A4" cell
worksheet.getCells().get("A4").putValue(200);
//Adding a sample value to "B1" cell
worksheet.getCells().get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.getCells().get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.getCells().get("B3").putValue(50);
//Adding a sample value to "B4" cell
worksheet.getCells().get("B4").putValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.getCells().get("C1").putValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.getCells().get("C2").putValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.getCells().get("C3").putValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.getCells().get("C4").putValue("Y2");
//Adding a chart to the worksheet
int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.getNSeries().add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.getNSeries().setCategoryData("C1:C4");
//adding a linear trendline
int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
//Setting the custom name of the trendline.
trendline.setName("Linear");
//Displaying the equation on chart
trendline.setDisplayEquation(true);
//Displaying the R-Squared value on chart
trendline.setDisplayRSquared(true);
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Specifies the length of the arrowhead for the begin of a line. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Specifies the width of the arrowhead for the begin of a line. |
| [getBeginType()](#getBeginType--) | Specifies an arrowhead for the begin of a line. |
| [getCapType()](#getCapType--) | Specifies the ending caps. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Represents the [Color](../../com.aspose.cells/color) of the line. |
| [getCompoundType()](#getCompoundType--) | Specifies the compound line type |
| [getDashType()](#getDashType--) | Specifies the dash line type |
| [getDataLabels()](#getDataLabels--) | Represents the DataLabels object for the specified series. |
| [getDisplayEquation()](#getDisplayEquation--) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). |
| [getDisplayRSquared()](#getDisplayRSquared--) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). |
| [getEndArrowLength()](#getEndArrowLength--) | Specifies the length of the arrowhead for the end of a line. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Specifies the width of the arrowhead for the end of a line. |
| [getEndType()](#getEndType--) | Specifies an arrowhead for the end of a line. |
| [getFormattingType()](#getFormattingType--) | Gets format type. |
| [getForward()](#getForward--) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. |
| [getGradientFill()](#getGradientFill--) | Represents gradient fill. |
| [getIntercept()](#getIntercept--) | Returns or sets the point where the trendline crosses the value axis. |
| [getJoinType()](#getJoinType--) | Specifies the joining caps. |
| [getLegendEntry()](#getLegendEntry--) | Gets the legend entry according to this trendline |
| [getName()](#getName--) | Returns the name of the trendline. |
| [getOrder()](#getOrder--) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. |
| [getPeriod()](#getPeriod--) | Returns or sets the period for the moving-average trendline. |
| [getStyle()](#getStyle--) | Represents the style of the line. |
| [getThemeColor()](#getThemeColor--) | Gets the theme color. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#getType--) | Returns the trendline type. |
| [getWeight()](#getWeight--) | Gets the [WeightType](../../com.aspose.cells/weighttype) of the line. |
| [getWeightPt()](#getWeightPt--) | Gets the weight of the line in unit of points. |
| [getWeightPx()](#getWeightPx--) | Gets the weight of the line in unit of pixels. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indicates whether this line style is auto assigned. |
| [isAutomaticColor()](#isAutomaticColor--) | Indicates whether the color of line is automatic assigned. |
| [isInterceptAuto()](#isInterceptAuto--) | Indicates whether Microsoft Workbook automatically determines the intercept of the trendline. |
| [isNameAuto()](#isNameAuto--) | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [isVisible()](#isVisible--) | Represents whether the line is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indicates whether this line style is auto assigned. |
| [setBackward(double value)](#setBackward-double-) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Specifies the length of the arrowhead for the begin of a line. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Specifies the width of the arrowhead for the begin of a line. |
| [setBeginType(int value)](#setBeginType-int-) | Specifies an arrowhead for the begin of a line. |
| [setCapType(int value)](#setCapType-int-) | Specifies the ending caps. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Represents the [Color](../../com.aspose.cells/color) of the line. |
| [setCompoundType(int value)](#setCompoundType-int-) | Specifies the compound line type |
| [setDashType(int value)](#setDashType-int-) | Specifies the dash line type |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Specifies the length of the arrowhead for the end of a line. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Specifies the width of the arrowhead for the end of a line. |
| [setEndType(int value)](#setEndType-int-) | Specifies an arrowhead for the end of a line. |
| [setFormattingType(int value)](#setFormattingType-int-) | Sets format type. |
| [setForward(double value)](#setForward-double-) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. |
| [setIntercept(double value)](#setIntercept-double-) | Returns or sets the point where the trendline crosses the value axis. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Sets whether Microsoft Workbook automatically determines the intercept of the trendline. |
| [setJoinType(int value)](#setJoinType-int-) | Specifies the joining caps. |
| [setName(String value)](#setName-java.lang.String-) | Returns the name of the trendline. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [setOrder(int value)](#setOrder-int-) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. |
| [setPeriod(int value)](#setPeriod-int-) | Returns or sets the period for the moving-average trendline. |
| [setStyle(int value)](#setStyle-int-) | Represents the style of the line. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Sets the theme color. |
| [setTransparency(double value)](#setTransparency-double-) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setVisible(boolean value)](#setVisible-boolean-) | Represents whether the line is visible. |
| [setWeight(int value)](#setWeight-int-) | Sets the [WeightType](../../com.aspose.cells/weighttype) of the line. |
| [setWeightPt(double value)](#setWeightPt-double-) | Sets the weight of the line in unit of points. |
| [setWeightPx(double value)](#setWeightPx-double-) | Sets the weight of the line in unit of pixels. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getBackward() {#getBackward--}
```
public double getBackward()
```
Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5
**Returns:**
double
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```
Specifies the length of the arrowhead for the begin of a line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```
Specifies the width of the arrowhead for the begin of a line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```
Specifies an arrowhead for the begin of a line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```
Specifies the ending caps.
See [LineCapType](../../com.aspose.cells/linecaptype).
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```
Represents the [Color](../../com.aspose.cells/color) of the line.
**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```
Specifies the compound line type
See [MsoLineStyle](../../com.aspose.cells/msolinestyle).
**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```
Specifies the dash line type
See [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).
**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```
Represents the DataLabels object for the specified series.
**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```
Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.
**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```
Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.
**Returns:**
boolean
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```
Specifies the length of the arrowhead for the end of a line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```
Specifies the width of the arrowhead for the end of a line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```
Specifies an arrowhead for the end of a line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```
Gets format type.
See [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).
**Returns:**
int
### getForward() {#getForward--}
```
public double getForward()
```
Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.
**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```
Represents gradient fill.
**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```
Returns or sets the point where the trendline crosses the value axis.
**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```
Specifies the joining caps.
See [LineJoinType](../../com.aspose.cells/linejointype).
**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```
Gets the legend entry according to this trendline
**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```
Returns the name of the trendline.
**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```
Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.
**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```
Returns or sets the period for the moving-average trendline.
**Remarks**
This value should be between 2 and 255. And it must be less than the number of the chart points in the series
**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```
Represents the style of the line.
See [LineType](../../com.aspose.cells/linetype).
**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```
Gets the theme color.
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```
Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).
**Returns:**
double
### getType() {#getType--}
```
public int getType()
```
Returns the trendline type.
See [TrendlineType](../../com.aspose.cells/trendlinetype).
**Returns:**
int
### getWeight() {#getWeight--}
```
public int getWeight()
```
Gets the [WeightType](../../com.aspose.cells/weighttype) of the line.
See [WeightType](../../com.aspose.cells/weighttype).
**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```
Gets the weight of the line in unit of points.
**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```
Gets the weight of the line in unit of pixels.
**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```
Indicates whether this line style is auto assigned.
**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```
Indicates whether the color of line is automatic assigned.
**Returns:**
boolean
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```
Indicates whether Microsoft Workbook automatically determines the intercept of the trendline.
**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```
Returns if Microsoft Excel automatically determines the name of the trendline.
**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```
Represents whether the line is visible.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```
Indicates whether this line style is auto assigned.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```
Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```
Specifies the length of the arrowhead for the begin of a line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```
Specifies the width of the arrowhead for the begin of a line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```
Specifies an arrowhead for the begin of a line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```
Specifies the ending caps.
See [LineCapType](../../com.aspose.cells/linecaptype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```
Represents the [Color](../../com.aspose.cells/color) of the line.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```
Specifies the compound line type
See [MsoLineStyle](../../com.aspose.cells/msolinestyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```
Specifies the dash line type
See [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```
Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```
Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```
Specifies the length of the arrowhead for the end of a line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```
Specifies the width of the arrowhead for the end of a line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```
Specifies an arrowhead for the end of a line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```
Sets format type.
See [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```
Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```
Returns or sets the point where the trendline crosses the value axis.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```
Sets whether Microsoft Workbook automatically determines the intercept of the trendline.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isInterceptAuto | boolean |  |
### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```
Specifies the joining caps.
See [LineJoinType](../../com.aspose.cells/linejointype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Returns the name of the trendline.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```
Returns if Microsoft Excel automatically determines the name of the trendline.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```
Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```
Returns or sets the period for the moving-average trendline.
**Remarks**
This value should be between 2 and 255. And it must be less than the number of the chart points in the series
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```
Represents the style of the line.
See [LineType](../../com.aspose.cells/linetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```
Sets the theme color.
**Remarks**
If the foreground color is not a theme color, NULL will be returned.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |
### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```
Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```
Represents whether the line is visible.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```
Sets the [WeightType](../../com.aspose.cells/weighttype) of the line.
See [WeightType](../../com.aspose.cells/weighttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```
Sets the weight of the line in unit of points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```
Sets the weight of the line in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
