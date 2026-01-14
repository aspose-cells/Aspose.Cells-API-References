---
title: Timeline
second_title: Aspose.Cells for Java API Reference
description: Summary description of Timeline View Due to MS Excel Excel 2003 does not support Timeline
type: docs
url: /java/com.aspose.cells/timeline/
---

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
| [getCaption()](#getCaption--) | Gets the caption of this Timeline. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | The current time level of the Timeline. |
| [getHeightPixel()](#getHeightPixel--) | Returns or sets the height of the specified timeline, in pixels. |
| [getLeftPixel()](#getLeftPixel--) | Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [getName()](#getName--) | Returns or sets the name of the specified Timeline |
| [getSelectionLevel()](#getSelectionLevel--) | Gets the time level at which the current selection was made for the Timeline. |
| [getShape()](#getShape--) | Returns the [TimelineShape](../../com.aspose.cells/timelineshape) object associated with this Timeline. |
| [getShowHeader()](#getShowHeader--) | Indicates whether to display the header. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Indicates whether to display the horizontal ccroll bar. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Indicates whether to display the selction label. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Indicates whether to display the time level. |
| [getStartDate()](#getStartDate--) | Gets the start date of the timespan scrolling position of this [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | Returns or sets the vertical offset of timeline shape from its top row, in pixels. |
| [getWidthPixel()](#getWidthPixel--) | Returns or sets the width of the specified timeline, in pixels. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaption(String value)](#setCaption-java.lang.String-) | Sets the caption of this Timeline. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | The current time level of the Timeline. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Returns or sets the height of the specified timeline, in pixels. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [setName(String value)](#setName-java.lang.String-) | Returns or sets the name of the specified Timeline |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Sets the time level at which the current selection was made for the Timeline. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Indicates whether to display the header. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Indicates whether to display the horizontal ccroll bar. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Indicates whether to display the selction label. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Indicates whether to display the time level. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Sets the start date of the timespan scrolling position of this [Timeline](../../com.aspose.cells/timeline). |
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


Gets the caption of this Timeline.

**Example**

```
         //Set the caption of this Timeline.
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
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


The current time level of the Timeline.

See [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
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
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Gets the time level at which the current selection was made for the Timeline.

See [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Returns the [TimelineShape](../../com.aspose.cells/timelineshape) object associated with this Timeline.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Indicates whether to display the header.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Indicates whether to display the horizontal ccroll bar.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Indicates whether to display the selction label.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Indicates whether to display the time level.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Gets the start date of the timespan scrolling position of this [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
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


Sets the caption of this Timeline.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


The current time level of the Timeline.

See [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Sets the time level at which the current selection was made for the Timeline.

See [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Indicates whether to display the header.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Indicates whether to display the horizontal ccroll bar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Indicates whether to display the selction label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Indicates whether to display the time level.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Sets the start date of the timespan scrolling position of this [Timeline](../../com.aspose.cells/timeline).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

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

