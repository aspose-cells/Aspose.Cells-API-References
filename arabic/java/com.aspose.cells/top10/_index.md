---
title: "Top10"
second_title: "Aspose.Cells for Java API Reference"
description: "وصف قاعدة التنسيق الشرطي Top10."
type: docs
url: /ar/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

وصف قاعدة التنسيق الشرطي Top10. تقوم هذه القاعدة بتسليط الضوء على الخلايا التي تقع قيمها في الفئة العليا N أو الفئة السفلى N، كما هو محدد.

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
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Top10()](#Top10--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | يحصل على قيمة "n" في قاعدة تنسيق شرطي "أعلى/أسفل n". |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | يُرجع ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n". |
| [isPercent()](#isPercent--) | يُرجع ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent". |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | يحدد ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n". |
| [setPercent(boolean value)](#setPercent-boolean-) | يحدد ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent". |
| [setRank(int value)](#setRank-int-) | يحدد قيمة "n" في قاعدة تنسيق شرطي "top/bottom n". |
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
| معامل | نوع | الوصف |
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


يُرجع قيمة "n" في قاعدة تنسيق شرطي "top/bottom n". إذا كان IsPercent صحيحًا، يجب أن تكون القيمة بين 0 و 100. وإلا يجب أن تكون بين 0 و 1000. القيمة الافتراضية هي 10.

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


يُرجع ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n". القيمة الافتراضية هي false.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


يُرجع ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent". القيمة الافتراضية هي false.

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


يحدد ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n". القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


يحدد ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent". القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


يحدد قيمة "n" في قاعدة تنسيق شرطي "top/bottom n". إذا كان IsPercent صحيحًا، يجب أن تكون القيمة بين 0 و 100. وإلا يجب أن تكون بين 0 و 1000. القيمة الافتراضية هي 10.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

