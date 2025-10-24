##ChartDataTable
Represents a chart data table.
**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```
Represents a chart data table.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a sample value to "B1" cell
worksheet.getCells().get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.getCells().get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.getCells().get("B3").putValue(50);
//Adding a chart to the worksheet
int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
//Accessing the instance of the newly added chart
Chart chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.getNSeries().add("A1:B3", true);
chart.setShowDataTable(true);
//Getting Chart Table
ChartDataTable chartTable = chart.getChartDataTable();
//Setting Chart Table Font Color
chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
//Setting Legend Key VisibilityOptions
chartTable.setShowLegendKey(false);
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | True if the text in the object changes font size when the object size changes. |
| [getBackgroundMode()](#getBackgroundMode--) | Gets the display mode of the background |
| [getBorder()](#getBorder--) | Returns a Border object that represents the border of the object |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object which represents the font setting of the specified chart data table. |
| [getShowLegendKey()](#getShowLegendKey--) | True if the data label legend key is visible. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | True if the chart data table has horizontal cell borders |
| [hasBorderOutline()](#hasBorderOutline--) | True if the chart data table has outline borders |
| [hasBorderVertical()](#hasBorderVertical--) | True if the chart data table has vertical cell borders |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | True if the chart data table has horizontal cell borders |
| [hasOutlineBorder()](#hasOutlineBorder--) | True if the chart data table has outline borders |
| [hasVerticalBorder()](#hasVerticalBorder--) | True if the chart data table has vertical cell borders |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True if the text in the object changes font size when the object size changes. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Sets the display mode of the background |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | True if the chart data table has horizontal cell borders |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | True if the chart data table has outline borders |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | True if the chart data table has vertical cell borders |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | True if the chart data table has horizontal cell borders |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | True if the chart data table has outline borders |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | True if the chart data table has vertical cell borders |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | True if the data label legend key is visible. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```
True if the text in the object changes font size when the object size changes. The default value is True.
**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```
Gets the display mode of the background
See [BackgroundMode](../../com.aspose.cells/backgroundmode).
**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```
Returns a Border object that represents the border of the object
**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```
Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object which represents the font setting of the specified chart data table.
**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```
True if the data label legend key is visible.
**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```
True if the chart data table has horizontal cell borders
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```
True if the chart data table has outline borders
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```
True if the chart data table has vertical cell borders
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```
True if the chart data table has horizontal cell borders
**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```
True if the chart data table has outline borders
**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```
True if the chart data table has vertical cell borders
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```
True if the text in the object changes font size when the object size changes. The default value is True.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```
Sets the display mode of the background
See [BackgroundMode](../../com.aspose.cells/backgroundmode).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```
True if the chart data table has horizontal cell borders
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```
True if the chart data table has outline borders
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```
True if the chart data table has vertical cell borders
**Remarks**
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```
True if the chart data table has horizontal cell borders
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```
True if the chart data table has outline borders
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```
True if the chart data table has vertical cell borders
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```
True if the data label legend key is visible.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
