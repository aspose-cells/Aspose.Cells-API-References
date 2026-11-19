---
title: "BorderCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

يحتوي على مجموعة من كائنات [Border](../../com.aspose.cells/border).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         Style style = cell.getStyle();
 
         //Setting the line style of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setColor(Color.getBlack());
 
         cell.setStyle(style);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | يحصل على عنصر [Border](../../com.aspose.cells/border) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | يحصل على [Color](../../com.aspose.cells/color) للخطوط القطرية. |
| [getDiagonalStyle()](#getDiagonalStyle--) | يحصل على نمط الخطوط القطرية. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | يشير إلى ما إذا كان يجب تطبيق الحدود اليسرى، اليمنى، العليا والسفلى فقط على حدود الخلية الخارجية لنطاق الخلايا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | يضبط [Color](../../com.aspose.cells/color) لجميع الحدود في المجموعة. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | يضبط [Color](../../com.aspose.cells/color) للخطوط القطرية. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | يضبط نمط الخطوط القطرية. |
| [setOutline(boolean value)](#setOutline-boolean-) | يشير إلى ما إذا كان يجب تطبيق الحدود اليسرى، اليمنى، العليا والسفلى فقط على حدود الخلية الخارجية لنطاق الخلايا. |
| [setStyle(int style)](#setStyle-int-) | يضبط نمط جميع الحدود في المجموعة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


يحصل على عنصر [Border](../../com.aspose.cells/border) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). الحد المراد استرجاعه. |

**Returns:**
[Border](../../com.aspose.cells/border) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDiagonalColor() {#getDiagonalColor--}
```
public Color getDiagonalColor()
```


يحصل على [Color](../../com.aspose.cells/color) للخطوط القطرية.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


يحصل على نمط الخطوط القطرية.

انظر [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


يشير إلى ما إذا كان يجب تطبيق الحدود اليسرى، اليمنى، العليا والسفلى فقط على حدود الخلية الخارجية لنطاق الخلايا. القيمة الافتراضية هي true.

**Remarks**

يعمل فقط عند تطبيقه على نطاق لتنسيقات شرطية أو جداول محورية. إذا كانت القيمة false، سيتم تطبيق الحدود اليسرى، اليمنى، العليا والسفلى على كل خلية، وإلا سيتم تطبيقها فقط على حدود الخلية الخارجية للنطاق. إذا كانت القيمة true، يرجى ضبط الحدود الأفقية والعمودية للحدود الداخلية للنطاق لتنسيقات شرطية أو جداول محورية.

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




### setColor(Color color) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color color)
```


يضبط [Color](../../com.aspose.cells/color) لجميع الحدود في المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | لون [Color](../../com.aspose.cells/color) للحدود. |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


يضبط [Color](../../com.aspose.cells/color) للخطوط القطرية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


يضبط نمط الخطوط القطرية.

انظر [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


يشير إلى ما إذا كان يجب تطبيق الحدود اليسرى، اليمنى، العليا والسفلى فقط على حدود الخلية الخارجية لنطاق الخلايا. القيمة الافتراضية هي true.

**Remarks**

يعمل فقط عند تطبيقه على نطاق لتنسيقات شرطية أو جداول محورية. إذا كانت القيمة false، سيتم تطبيق الحدود اليسرى، اليمنى، العليا والسفلى على كل خلية، وإلا سيتم تطبيقها فقط على حدود الخلية الخارجية للنطاق. إذا كانت القيمة true، يرجى ضبط الحدود الأفقية والعمودية للحدود الداخلية للنطاق لتنسيقات شرطية أو جداول محورية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


يضبط نمط جميع الحدود في المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحدود |

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

