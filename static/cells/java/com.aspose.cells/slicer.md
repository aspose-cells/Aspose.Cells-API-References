##Slicer
summary description of Slicer View
**Inheritance:**
java.lang.Object
```
public class Slicer
```
summary description of Slicer View
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
cells.get(5, 0).setValue("grape");
cells.get(6, 0).setValue("blueberry");
cells.get(7, 0).setValue("kiwi");
cells.get(8, 0).setValue("cherry");
cells.get(0, 1).setValue("year");
cells.get(1, 1).setValue(2020);
cells.get(2, 1).setValue(2020);
cells.get(3, 1).setValue(2020);
cells.get(4, 1).setValue(2020);
cells.get(5, 1).setValue(2021);
cells.get(6, 1).setValue(2021);
cells.get(7, 1).setValue(2021);
cells.get(8, 1).setValue(2021);
cells.get(0, 2).setValue("amount");
cells.get(1, 2).setValue(50);
cells.get(2, 2).setValue(60);
cells.get(3, 2).setValue(70);
cells.get(4, 2).setValue(80);
cells.get(5, 2).setValue(90);
cells.get(6, 2).setValue(100);
cells.get(7, 2).setValue(110);
cells.get(8, 2).setValue(120);
PivotTableCollection pivots = sheet.getPivotTables();
int pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots.get(pivotIndex);
pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
pivot.addFieldToArea(PivotFieldType.DATA, "amount");
pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
pivot.refreshData();
pivot.calculateData();
SlicerCollection slicers = sheet.getSlicers();
int slicerIndex = slicers.add(pivot, "E12", "fruit");
Slicer slicer = slicers.get(slicerIndex);
slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
SlicerCacheItemCollection items = slicer.getSlicerCache().getSlicerCacheItems();
SlicerCacheItem item = items.get(0);
item.setSelected(false);
//do your business
book.save("out.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | Adds PivotTable connection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [getCaption()](#getCaption--) | Returns or sets the caption of the specified slicer. |
| [getCaptionVisible()](#getCaptionVisible--) | Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Returns or sets the width, in points, of each column in the slicer. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Gets the width of\\u807deach column in\\u807dthe slicer, in unit of\\u807dpixels.\\u807d |
| [getHeight()](#getHeight--) | Returns or sets the height of the specified slicer, in points. |
| [getHeightPixel()](#getHeightPixel--) | Returns or sets the height of the specified slicer, in pixels. |
| [getLeftPixel()](#getLeftPixel--) | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | Indicates whether locking aspect ratio. |
| [getLockedPosition()](#getLockedPosition--) | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [getName()](#getName--) | Returns or sets the name of the specified slicer |
| [getNumberOfColumns()](#getNumberOfColumns--) | Returns or sets the number of columns in the specified slicer. |
| [getParent()](#getParent--) | Returns the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object which contains this slicer. |
| [getPlacement()](#getPlacement--) | Represents the way the drawing object is attached to the cells below it. |
| [getRowHeight()](#getRowHeight--) | Returns or sets the height, in points, of each row in the specified slicer. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Returns or sets the height, in pixels, of each row in the specified slicer. |
| [getShape()](#getShape--) | Returns the Shape object associated with the specified slicer. |
| [getSlicerCache()](#getSlicerCache--) | Returns the SlicerCache object associated with the slicer. |
| [getStyleType()](#getStyleType--) | Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [getTitle()](#getTitle--) | Specifies the title of the current Slicer object. |
| [getTopPixel()](#getTopPixel--) | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [getWidth()](#getWidth--) | Returns or sets the width of the specified slicer, in points. |
| [getWidthPixel()](#getWidthPixel--) | Returns or sets the width of the specified slicer, in pixels. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Indicates whether the slicer shape is locked. |
| [isPrintable()](#isPrintable--) | Indicates whether the slicer object is printable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Refreshing the slicer.Meanwhile, Refreshing and Calculating relative PivotTables. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | Removes PivotTable connection. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Returns or sets the caption of the specified slicer. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Returns or sets the width, in points, of each column in the slicer. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Sets the width of\\u807deach column in\\u807dthe slicer, in unit of\\u807dpixels.\\u807d |
| [setHeight(double value)](#setHeight-double-) | Returns or sets the height of the specified slicer, in points. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Returns or sets the height of the specified slicer, in pixels. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indicates whether the slicer shape is locked. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | Indicates whether locking aspect ratio. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [setName(String value)](#setName-java.lang.String-) | Returns or sets the name of the specified slicer |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Returns or sets the number of columns in the specified slicer. |
| [setPlacement(int value)](#setPlacement-int-) | Represents the way the drawing object is attached to the cells below it. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indicates whether the slicer object is printable. |
| [setRowHeight(double value)](#setRowHeight-double-) | Returns or sets the height, in points, of each row in the specified slicer. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Returns or sets the height, in pixels, of each row in the specified slicer. |
| [setStyleType(int value)](#setStyleType-int-) | Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [setTitle(String value)](#setTitle-java.lang.String-) | Specifies the title of the current Slicer object. |
| [setTopPixel(int value)](#setTopPixel-int-) | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [setWidth(double value)](#setWidth-double-) | Returns or sets the width of the specified slicer, in points. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Returns or sets the width of the specified slicer, in pixels. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```
Adds PivotTable connection.
**Example**
```
slicer.addPivotConnection(pivot);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | The PivotTable object |
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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```
Returns or sets the descriptive (alternative) text string of the Slicer object.
**Example**
```
slicer.setAlternativeText("AlternativeText test");
```
**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```
Returns or sets the caption of the specified slicer.
**Example**
```
slicer.setCaption("slicer caption");
```
**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```
Returns or sets whether the header that displays the slicer Caption is visible the default value is true
**Example**
```
slicer.setCaptionVisible(true);
```
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```
Returns or sets the width, in points, of each column in the slicer.
**Example**
```
slicer.setColumnWidth(80);
```
**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```
Gets the width of\\u807deach column in\\u807dthe slicer, in unit of\\u807dpixels.\\u807d
**Example**
```
slicer.setColumnWidthPixel(120);
```
**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```
Returns or sets the height of the specified slicer, in points.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.HeightPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Example**
```
slicer.setNumberOfColumns(1);
```
**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```
Returns or sets the height of the specified slicer, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Example**
```
slicer.setNumberOfColumns(1);
```
**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```
Returns or sets the horizontal offset of slicer shape from its left column, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Example**
```
slicer.setNumberOfColumns(1);
```
**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```
Indicates whether locking aspect ratio.
**Example**
```
slicer.setLockedAspectRatio(true);
```
**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```
Indicates whether the specified slicer can be moved or resized by using the user interface.
**Example**
```
slicer.setLockedPosition(false);
```
**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```
Returns or sets the name of the specified slicer
**Example**
```
slicer.setName("slicer name");
```
**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```
Returns or sets the number of columns in the specified slicer.
**Example**
```
slicer.setNumberOfColumns(1);
```
**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```
Returns the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object which contains this slicer. Read-only.
**Example**
```
Worksheet currSheet = slicer.getParent();
```
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```
Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.
See [PlacementType](../../com.aspose.cells/placementtype).
**Example**
```
slicer.setPlacement(PlacementType.FREE_FLOATING);
```
**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```
Returns or sets the height, in points, of each row in the specified slicer.
**Example**
```
slicer.setRowHeight(20);
```
**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```
Returns or sets the height, in pixels, of each row in the specified slicer.
**Example**
```
slicer.setRowHeightPixel(30);
```
**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```
Returns the Shape object associated with the specified slicer. Read-only.
**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```
Returns the SlicerCache object associated with the slicer. Read-only.
**Example**
```
SlicerCache slicerCache = slicer.getSlicerCache();
```
**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```
Specify the type of Built-in slicer style the default type is SlicerStyleLight1
See [SlicerStyleType](../../com.aspose.cells/slicerstyletype).
**Example**
```
slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```
**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```
Specifies the title of the current Slicer object.
**Example**
```
slicer.setTitle("slicer title");
```
**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```
Returns or sets the vertical offset of slicer shape from its top row, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Example**
```
slicer.setNumberOfColumns(1);
```
**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```
Returns or sets the width of the specified slicer, in points.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.WidthPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Example**
```
slicer.setNumberOfColumns(1);
```
**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```
Returns or sets the width of the specified slicer, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Example**
```
slicer.setNumberOfColumns(1);
```
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```
Indicates whether the slicer shape is locked.
**Example**
```
slicer.setLocked(false);
```
**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```
Indicates whether the slicer object is printable.
**Example**
```
slicer.setPrintable(true);
```
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
### refresh() {#refresh--}
```
public void refresh()
```
Refreshing the slicer.Meanwhile, Refreshing and Calculating relative PivotTables.
**Example**
```
slicer.refresh();
```
### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```
Removes PivotTable connection.
**Example**
```
slicer.removePivotConnection(pivot);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | The PivotTable object |
### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```
Returns or sets the descriptive (alternative) text string of the Slicer object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```
Returns or sets the caption of the specified slicer.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```
Returns or sets whether the header that displays the slicer Caption is visible the default value is true
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```
Returns or sets the width, in points, of each column in the slicer.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```
Sets the width of\\u807deach column in\\u807dthe slicer, in unit of\\u807dpixels.\\u807d
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```
Returns or sets the height of the specified slicer, in points.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.HeightPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```
Returns or sets the height of the specified slicer, in pixels.
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
Returns or sets the horizontal offset of slicer shape from its left column, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```
Indicates whether the slicer shape is locked.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```
Indicates whether locking aspect ratio.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```
Indicates whether the specified slicer can be moved or resized by using the user interface.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Returns or sets the name of the specified slicer
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```
Returns or sets the number of columns in the specified slicer.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```
Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.
See [PlacementType](../../com.aspose.cells/placementtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```
Indicates whether the slicer object is printable.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```
Returns or sets the height, in points, of each row in the specified slicer.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```
Returns or sets the height, in pixels, of each row in the specified slicer.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```
Specify the type of Built-in slicer style the default type is SlicerStyleLight1
See [SlicerStyleType](../../com.aspose.cells/slicerstyletype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```
Specifies the title of the current Slicer object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```
Returns or sets the vertical offset of slicer shape from its top row, in pixels.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```
Returns or sets the width of the specified slicer, in points.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.WidthPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```
Returns or sets the width of the specified slicer, in pixels.
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
