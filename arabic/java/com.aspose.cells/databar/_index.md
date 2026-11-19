---
title: "DataBar"
second_title: "Aspose.Cells for Java API Reference"
description: "وصف قاعدة تنسيق الشرط للـ DataBar."
type: docs
url: /ar/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

صف قاعدة تنسيق الخلايا الشرطية DataBar. تعرض قاعدة تنسيق الخلايا الشرطية هذه شريط بيانات متدرج في نطاق الخلايا.

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
         int idx = fcs.addCondition(FormatConditionType.DATA_BAR);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Databar
         DataBar dataBar = cond.getDataBar();
 
         dataBar.setColor(Color.getOrange());
 
         //Set Databar properties
         dataBar.getMinCfvo().setType(FormatConditionValueType.PERCENTILE);
 
         dataBar.getMinCfvo().setValue(30);
 
         dataBar.setShowValue(false);
 
         dataBar.getBarBorder().setType(DataBarBorderType.SOLID);
 
         dataBar.getBarBorder().setColor(Color.getPlum());
 
          dataBar.setBarFillType(DataBarFillType.SOLID);
 
          dataBar.setAxisColor(Color.getRed());
 
          dataBar.setAxisPosition(DataBarAxisPosition.MIDPOINT);
 
          dataBar.getNegativeBarFormat().setColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setColor(Color.getWhite());
 
          dataBar.getNegativeBarFormat().setBorderColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setBorderColor(Color.getYellow());
 
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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | يحصل على لون المحور للخلايا التي تم تنسيقها شرطياً كشريط بيانات. |
| [getAxisPosition()](#getAxisPosition--) | يحصل على موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق خلايا شرطية. |
| [getBarBorder()](#getBarBorder--) | يحصل على كائن يحدد حدود شريط البيانات. |
| [getBarFillType()](#getBarFillType--) | يحصل على طريقة تعبئة شريط البيانات باللون. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يحصل على لون هذا DataBar. |
| [getDirection()](#getDirection--) | يحصل على اتجاه عرض شريط البيانات. |
| [getMaxCfvo()](#getMaxCfvo--) | يحصل على كائن القيمة القصوى لهذا DataBar. |
| [getMaxLength()](#getMaxLength--) | يمثل الحد الأقصى لطول شريط البيانات. |
| [getMinCfvo()](#getMinCfvo--) | يحصل على كائن القيمة الدنيا لهذا DataBar. |
| [getMinLength()](#getMinLength--) | يمثل الحد الأدنى لطول شريط البيانات. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | يحصل على كائن NegativeBarFormat المرتبط بقاعدة تنسيق خلايا شرطية لشريط البيانات. |
| [getShowValue()](#getShowValue--) | يحصل على العلامة التي تشير إلى ما إذا كان يجب عرض قيم الخلايا التي تم تطبيق شريط البيانات عليها. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | يحصل على لون المحور للخلايا التي تم تنسيقها شرطياً كشريط بيانات. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | يضبط موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق خلايا شرطية. |
| [setBarFillType(int value)](#setBarFillType-int-) | يضبط طريقة تعبئة شريط البيانات باللون. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يضبط لون هذا DataBar. |
| [setDirection(int value)](#setDirection-int-) | يضبط اتجاه عرض شريط البيانات. |
| [setMaxLength(int value)](#setMaxLength-int-) | يمثل الحد الأقصى لطول شريط البيانات. |
| [setMinLength(int value)](#setMinLength-int-) | يمثل الحد الأدنى لطول شريط البيانات. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | يضبط العلامة التي تشير إلى ما إذا كان يجب عرض قيم الخلايا التي تم تطبيق شريط البيانات عليها. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | تحويل شريط البيانات في الخلية إلى مصفوفة بايت للصورة. |
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
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


يحصل على لون المحور للخلايا التي تم تنسيقها شرطياً كشريط بيانات.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


يحصل على موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق خلايا شرطية.

انظر [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


يحصل على كائن يحدد حدود شريط البيانات.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


يحصل على طريقة تعبئة شريط البيانات باللون.

انظر [DataBarFillType](../../com.aspose.cells/databarfilltype).

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


يحصل على لون هذا DataBar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


يحصل على اتجاه عرض شريط البيانات.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


يحصل على كائن القيمة القصوى لهذا DataBar. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Min إليه.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


يمثل الحد الأقصى لطول شريط البيانات.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


يحصل على كائن القيمة الدنيا لهذا DataBar. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


يمثل الحد الأدنى لطول شريط البيانات.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


يحصل على كائن NegativeBarFormat المرتبط بقاعدة تنسيق خلايا شرطية لشريط البيانات.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


يحصل على العلامة التي تشير إلى ما إذا كان يجب عرض قيم الخلايا التي تم تطبيق شريط البيانات عليها. القيمة الافتراضية هي true.

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




### setAxisColor(Color value) {#setAxisColor-com.aspose.cells.Color-}
```
public void setAxisColor(Color value)
```


يحصل على لون المحور للخلايا التي تم تنسيقها شرطياً كشريط بيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


يضبط موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق خلايا شرطية.

انظر [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


يضبط طريقة تعبئة شريط البيانات باللون.

انظر [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


يضبط لون هذا DataBar.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


يضبط اتجاه عرض شريط البيانات.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


يمثل الحد الأقصى لطول شريط البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


يمثل الحد الأدنى لطول شريط البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


يضبط العلامة التي تشير إلى ما إذا كان يجب عرض قيم الخلايا التي يُطبق عليها شريط البيانات هذا. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


تحويل شريط البيانات في الخلية إلى مصفوفة بايت للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | حدد شريط البيانات في الخلية التي يجب عرضها |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions يحتوي على بعض خصائص الصورة الناتجة |

**Returns:**
byte[] -
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

