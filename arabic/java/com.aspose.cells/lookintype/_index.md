---
title: "LookInType"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل نوع النظرة داخل."
type: docs
url: /ar/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

يمثل نوع النظرة داخل.
## حقول

| حقل | الوصف |
| --- | --- |
| [COMMENTS](#COMMENTS) | يبحث عن الكائن من تعليق الخلية فقط. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | ابحث عن الكائن من القيمة المنسقة للخلية([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) فقط. |
| [FORMULAS](#FORMULAS) | يبحث عن الكائن المطلوب من الصيغة([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) إذا كانت الخلية صيغة، وإلا يبحث من القيمة الأصلية للخلية (نفس ما هو في [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | يتجاهل الخلايا التي ليست صيغًا. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | ابحث عن الكائن من القيمة الأصلية للخلية فقط. |
| [VALUES](#VALUES) | يبحث عن الكائن من القيمة الأصلية للخلية([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) والقيمة المنسقة([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | يتجاهل الخلايا التي هي صيغ. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


يبحث عن الكائن من تعليق الخلية فقط. يتجاهل تلك الخلايا التي لا تحتوي على تعليق.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


ابحث عن الكائن من القيمة المنسقة للخلية([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) فقط.

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


يبحث عن الكائن المطلوب من الصيغة([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) إذا كانت الخلية صيغة، وإلا يبحث من القيمة الأصلية للخلية (نفس ما هو في [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


يتجاهل الخلايا التي ليست صيغًا. بالنسبة لتلك الخلايا التي هي صيغ، يبحث عن الكائن المطلوب من الصيغة([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)).

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


ابحث عن الكائن من القيمة الأصلية للخلية فقط.

### VALUES {#VALUES}
```
public static final int VALUES
```


يبحث عن الكائن من القيمة الأصلية للخلية([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) والقيمة المنسقة([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


يتجاهل الخلايا التي هي صيغ. بالنسبة لتلك الخلايا التي ليست صيغًا، يكون الأمر نفسه مع [VALUES](../../com.aspose.cells/lookintype\#VALUES).

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

