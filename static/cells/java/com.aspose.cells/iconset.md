##IconSet
Describe the IconSet conditional formatting rule.
**Inheritance:**
java.lang.Object
```
public class IconSet
```
Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.getWorksheets().get(0);
//Adds an empty conditional formatting
int index = sheet.getConditionalFormattings().add();
FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
//Sets the conditional format range.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 2;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.addArea(ca);
//Adds condition.
int idx = fcs.addCondition(FormatConditionType.ICON_SET);
fcs.addArea(ca);
FormatCondition cond = fcs.get(idx);
//Get Icon Set
IconSet iconSet = cond.getIconSet();
//Set Icon Type
iconSet.setType(IconSetType.ARROWS_3);
//Put Cell Values
Cell cell1 = sheet.getCells().get("A1");
cell1.putValue(10);
Cell cell2 = sheet.getCells().get("A2");
cell2.putValue(120);
Cell cell3 = sheet.getCells().get("A3");
cell3.putValue(260);
//Saving the Excel file
workbook.save("book1.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Get the[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) from the collection |
| [getCfvos()](#getCfvos--) | Get the CFValueObjects instance. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Gets the flag indicating whether to reverses the default order of the icons in this icon set. |
| [getShowValue()](#getShowValue--) | Gets the flag indicating whether to show the values of the cells on which this icon set is applied. |
| [getType()](#getType--) | Gets the icon set type to display. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Indicates whether the icon set is custom. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Sets the flag indicating whether to reverses the default order of the icons in this icon set. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Sets the flag indicating whether to show the values of the cells on which this icon set is applied. |
| [setType(int value)](#setType-int-) | Sets the icon set type to display. |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```
Get the[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) from the collection
**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```
Get the CFValueObjects instance.
**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```
Gets the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.
**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```
Gets the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.
**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```
Gets the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.
See [IconSetType](../../com.aspose.cells/iconsettype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```
Indicates whether the icon set is custom. Default value is false.
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
### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```
Sets the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```
Sets the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setType(int value) {#setType-int-}
```
public void setType(int value)
```
Sets the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.
See [IconSetType](../../com.aspose.cells/iconsettype).
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
