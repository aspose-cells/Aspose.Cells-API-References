##Timeline
Summary description of Timeline View Due to MS Excel Excel 2003 does not support Timeline
**Inheritance:**
java.lang.Object
```
public class Timeline
```
Summary description of Timeline View Due to MS Excel, Excel 2003 does not support Timeline
**Example**
```
Workbook book = new Workbook();
Worksheet sheet = book.getWorksheets().get(0);
Cells cells = sheet.getCells();
cells.get(0, 0).setValue("fruit");
cells.get(1, 0).setValue("grape");
cells.get(2, 0).setValue("blueberry");
cells.get(3, 0).setValue("kiwi");
cells.get(4, 0).setValue("cherry");
//Create date style
Style dateStyle = new CellsFactory().createStyle();
dateStyle.setCustom("m/d/yyyy");
cells.get(0, 1).setValue("date");
cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
//Set date style
cells.get(1, 1).setStyle(dateStyle);
cells.get(2, 1).setStyle(dateStyle);
cells.get(3, 1).setStyle(dateStyle);
cells.get(4, 1).setStyle(dateStyle);
cells.get(0, 2).setValue("amount");
cells.get(1, 2).setValue(50);
cells.get(2, 2).setValue(60);
cells.get(3, 2).setValue(70);
cells.get(4, 2).setValue(80);
PivotTableCollection pivots = sheet.getPivotTables();
//Add a PivotTable
int pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable");
PivotTable pivot = pivots.get(pivotIndex);
pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
pivot.addFieldToArea(PivotFieldType.DATA, "amount");
pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
//Refresh PivotTable data
pivot.refreshData();
pivot.calculateData();
//Add a new Timeline using PivotTable as data source
sheet.getTimelines().add(pivot, 10, 5, "date");
//Get Timeline object
Timeline timelineObj = sheet.getTimelines().get(0);
//do your business
book.save("out.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Returns or sets the caption of the specified Timeline. |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Returns or sets the height of the specified timeline, in pixels. |
| [getLeftPixel()](#getLeftPixel--) | Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [getName()](#getName--) | Returns or sets the name of the specified Timeline |
| [getShape()](#getShape--) | Returns the [TimelineShape](../../com.aspose.cells/timelineshape) object associated with this Timeline. |
| [getTopPixel()](#getTopPixel--) | Returns or sets the vertical offset of timeline shape from its top row, in pixels. |
| [getWidthPixel()](#getWidthPixel--) | Returns or sets the width of the specified timeline, in pixels. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaption(String value)](#setCaption-java.lang.String-) | Returns or sets the caption of the specified Timeline. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Returns or sets the height of the specified timeline, in pixels. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [setName(String value)](#setName-java.lang.String-) | Returns or sets the name of the specified Timeline |
| [setTopPixel(int value)](#setTopPixel-int-) | Returns or sets the vertical offset of timeline shape from its top row, in pixels. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Returns or sets the width of the specified timeline, in pixels. |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```
Returns or sets the caption of the specified Timeline.
**Example**
```
//Set the caption of the specified Timeline.
timelineObj.setCaption("timeline caption test");
```
**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```
Returns or sets the height of the specified timeline, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```
Returns or sets the horizontal offset of timeline shape from its left column, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getName() {#getName--}
```
public String getName()
```
Returns or sets the name of the specified Timeline
**Example**
```
//Set the name of the specified Timeline.
timelineObj.setName("timeline name test");
```
**Returns:**
java.lang.String
### getShape() {#getShape--}
```
public TimelineShape getShape()
```
Returns the [TimelineShape](../../com.aspose.cells/timelineshape) object associated with this Timeline. Read-only.
**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```
Returns or sets the vertical offset of timeline shape from its top row, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```
Returns or sets the width of the specified timeline, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
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
### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```
Returns or sets the caption of the specified Timeline.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```
Returns or sets the height of the specified timeline, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```
Returns or sets the horizontal offset of timeline shape from its left column, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Returns or sets the name of the specified Timeline
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```
Returns or sets the vertical offset of timeline shape from its top row, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```
Returns or sets the width of the specified timeline, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
