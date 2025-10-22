##Top10
Describe the Top10 conditional formatting rule.
**Inheritance:**
java.lang.Object
```
public class Top10
```
Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.getWorksheets().get(0);
//Adds an empty conditional formatting
int index = sheet.getConditionalFormattings().add();
FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
//Sets the conditional format range.
CellArea ca = CellArea.createCellArea(0, 0, 10, 10);
fcs.addArea(ca);
//Adds condition.
int conditionIndex = fcs.addCondition(FormatConditionType.TOP_10, OperatorType.NONE, null, null);
//Sets the background color.
FormatCondition fc = fcs.get(conditionIndex);
fc.getStyle().setBackgroundColor(Color.getRed());
Top10 top10 = fc.getTop10();
//Set the Top N
top10.setRank(5);
//Saving the Excel file
workbook.save("output.xls");
```
## Constructors
| Constructor | Description |
| --- | --- |
| [Top10()](#Top10--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Gets the value of "n" in a "top/bottom n" conditional formatting rule. |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Gets whether a "top/bottom n" rule is a "bottom n" rule. |
| [isPercent()](#isPercent--) | Gets whether a "top/bottom n" rule is a "top/bottom n percent" rule. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Sets whether a "top/bottom n" rule is a "bottom n" rule. |
| [setPercent(boolean value)](#setPercent-boolean-) | Sets whether a "top/bottom n" rule is a "top/bottom n percent" rule. |
| [setRank(int value)](#setRank-int-) | Sets the value of "n" in a "top/bottom n" conditional formatting rule. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Top10() {#Top10--}
```
public Top10()
```
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getRank() {#getRank--}
```
public int getRank()
```
Gets the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isBottom() {#isBottom--}
```
public boolean isBottom()
```
Gets whether a "top/bottom n" rule is a "bottom n" rule. Default value is false.
**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```
Gets whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false.
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
### setBottom(boolean value) {#setBottom-boolean-}
```
public void setBottom(boolean value)
```
Sets whether a "top/bottom n" rule is a "bottom n" rule. Default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```
Sets whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```
Sets the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10.
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
