##ErrorBar
Represents error bar of data series.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```
Represents error bar of data series.
**Example**
```
Workbook workbook = new Workbook();
Cells cells = workbook.getWorksheets().get(0).getCells();
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
int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 11, 0, 27, 10);
Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
chart.getNSeries().add("A1:B4", true);
chart.getNSeries().setCategoryData("C1:C4");
for(int i = 0; i <chart.getNSeries().getCount(); i ++)
{
Series aseries = chart.getNSeries().get(i);
aseries.getYErrorBar().setDisplayType(ErrorBarDisplayType.MINUS);
aseries.getYErrorBar().setType(ErrorBarType.FIXED_VALUE);
aseries.getYErrorBar().setAmount(5);
}
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | Represents amount of error bar. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Specifies the length of the arrowhead for the begin of a line. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Specifies the width of the arrowhead for the begin of a line. |
| [getBeginType()](#getBeginType--) | Specifies an arrowhead for the begin of a line. |
| [getCapType()](#getCapType--) | Specifies the ending caps. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Represents the [Color](../../com.aspose.cells/color) of the line. |
| [getCompoundType()](#getCompoundType--) | Specifies the compound line type |
| [getDashType()](#getDashType--) | Specifies the dash line type |
| [getDisplayType()](#getDisplayType--) | Represents the display type of error bar. |
| [getEndArrowLength()](#getEndArrowLength--) | Specifies the length of the arrowhead for the end of a line. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Specifies the width of the arrowhead for the end of a line. |
| [getEndType()](#getEndType--) | Specifies an arrowhead for the end of a line. |
| [getFormattingType()](#getFormattingType--) | Gets format type. |
| [getGradientFill()](#getGradientFill--) | Represents gradient fill. |
| [getJoinType()](#getJoinType--) | Specifies the joining caps. |
| [getMinusValue()](#getMinusValue--) | Represents negative error amount when error bar type is Custom. |
| [getPlusValue()](#getPlusValue--) | Represents positive error amount when error bar type is Custom. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | Indicates if formatting error bars with a T-top. |
| [getStyle()](#getStyle--) | Represents the style of the line. |
| [getThemeColor()](#getThemeColor--) | Gets the theme color. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#getType--) | Represents error bar amount type. |
| [getWeight()](#getWeight--) | Gets the [WeightType](../../com.aspose.cells/weighttype) of the line. |
| [getWeightPt()](#getWeightPt--) | Gets the weight of the line in unit of points. |
| [getWeightPx()](#getWeightPx--) | Gets the weight of the line in unit of pixels. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indicates whether this line style is auto assigned. |
| [isAutomaticColor()](#isAutomaticColor--) | Indicates whether the color of line is automatic assigned. |
| [isVisible()](#isVisible--) | Represents whether the line is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | Represents amount of error bar. |
| [setAuto(boolean value)](#setAuto-boolean-) | Indicates whether this line style is auto assigned. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Specifies the length of the arrowhead for the begin of a line. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Specifies the width of the arrowhead for the begin of a line. |
| [setBeginType(int value)](#setBeginType-int-) | Specifies an arrowhead for the begin of a line. |
| [setCapType(int value)](#setCapType-int-) | Specifies the ending caps. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Represents the [Color](../../com.aspose.cells/color) of the line. |
| [setCompoundType(int value)](#setCompoundType-int-) | Specifies the compound line type |
| [setDashType(int value)](#setDashType-int-) | Specifies the dash line type |
| [setDisplayType(int value)](#setDisplayType-int-) | Represents the display type of error bar. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Specifies the length of the arrowhead for the end of a line. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Specifies the width of the arrowhead for the end of a line. |
| [setEndType(int value)](#setEndType-int-) | Specifies an arrowhead for the end of a line. |
| [setFormattingType(int value)](#setFormattingType-int-) | Sets format type. |
| [setJoinType(int value)](#setJoinType-int-) | Specifies the joining caps. |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | Represents negative error amount when error bar type is Custom. |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | Represents positive error amount when error bar type is Custom. |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | Indicates if formatting error bars with a T-top. |
| [setStyle(int value)](#setStyle-int-) | Represents the style of the line. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Sets the theme color. |
| [setTransparency(double value)](#setTransparency-double-) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setType(int value)](#setType-int-) | Represents error bar amount type. |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```
Represents amount of error bar.
**Remarks**
The amount must be greater than or equal to zero.
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
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```
Represents the display type of error bar.
See [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).
**Returns:**
int
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
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```
Represents gradient fill.
**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```
Specifies the joining caps.
See [LineJoinType](../../com.aspose.cells/linejointype).
**Returns:**
int
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```
Represents negative error amount when error bar type is Custom.
**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```
Represents positive error amount when error bar type is Custom.
**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```
Indicates if formatting error bars with a T-top.
**Returns:**
boolean
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
Represents error bar amount type.
See [ErrorBarType](../../com.aspose.cells/errorbartype).
**Example**
```
Workbook wb = new Workbook("chart.xlsx");
Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
Series aseries = chart.getNSeries().get(0);
//Sets custom error bar type
aseries.getYErrorBar().setType(ErrorBarType.CUSTOM);
aseries.getYErrorBar().setPlusValue("=Sheet1!A1");
aseries.getYErrorBar().setMinusValue("=Sheet1!A2");
```
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
### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```
Represents amount of error bar.
**Remarks**
The amount must be greater than or equal to zero.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```
Indicates whether this line style is auto assigned.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```
Represents the display type of error bar.
See [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```
Represents negative error amount when error bar type is Custom.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```
Represents positive error amount when error bar type is Custom.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```
Indicates if formatting error bars with a T-top.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
### setType(int value) {#setType-int-}
```
public void setType(int value)
```
Represents error bar amount type.
See [ErrorBarType](../../com.aspose.cells/errorbartype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
