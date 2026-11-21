---
title: "DataBar"
second_title: "Aspose.Cells for Java API Referansı"
description: "DataBar koşullu biçimlendirme kuralını tanımlar."
type: docs
url: /tr/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

DataBar koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, hücre aralığında dereceli bir veri çubuğu gösterir.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | Koşullu biçimlendirmeye sahip hücreler için eksenin rengini alır. |
| [getAxisPosition()](#getAxisPosition--) | Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının eksen konumunu alır. |
| [getBarBorder()](#getBarBorder--) | Bir veri çubuğunun kenarlığını belirten nesneyi alır. |
| [getBarFillType()](#getBarFillType--) | Bir veri çubuğunun renk ile nasıl doldurulduğunu alır. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Bu DataBar'ın Rengini alır. |
| [getDirection()](#getDirection--) | Veri çubuğunun görüntülendiği yönü alır. |
| [getMaxCfvo()](#getMaxCfvo--) | Bu DataBar'ın maksimum değer nesnesini alır. |
| [getMaxLength()](#getMaxLength--) | Veri çubuğunun maksimum uzunluğunu temsil eder. |
| [getMinCfvo()](#getMinCfvo--) | Bu DataBar'ın minimum değer nesnesini alır. |
| [getMinLength()](#getMinLength--) | Veri çubuğunun minimum uzunluğunu temsil eder. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Bir veri çubuğu koşullu biçimlendirme kuralı ile ilişkili NegativeBarFormat nesnesini alır. |
| [getShowValue()](#getShowValue--) | Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Koşullu biçimlendirmeye sahip hücreler için eksenin rengini alır. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının eksen konumunu ayarlar. |
| [setBarFillType(int value)](#setBarFillType-int-) | Bir veri çubuğunun renk ile nasıl doldurulacağını ayarlar. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Bu DataBar'ın Rengini ayarlar. |
| [setDirection(int value)](#setDirection-int-) | Veri çubuğunun görüntülendiği yönü ayarlar. |
| [setMaxLength(int value)](#setMaxLength-int-) | Veri çubuğunun maksimum uzunluğunu temsil eder. |
| [setMinLength(int value)](#setMinLength-int-) | Veri çubuğunun minimum uzunluğunu temsil eder. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı ayarlar. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Hücredeki veri çubuğunu görüntü bayt dizisine render eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


Koşullu biçimlendirmeye sahip hücreler için eksenin rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının eksen konumunu alır.

Bakınız [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


Bir veri çubuğunun kenarlığını belirten nesneyi alır.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


Bir veri çubuğunun renk ile nasıl doldurulduğunu alır.

Bakınız [DataBarFillType](../../com.aspose.cells/databarfilltype).

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


Bu DataBar'ın Rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


Veri çubuğunun görüntülendiği yönü alır.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Bu DataBar'ın maksimum değer nesnesini alır. Buna null veya FormatConditionValueType.Min tipinde CFValueObject atanamaz.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Veri çubuğunun maksimum uzunluğunu temsil eder.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Bu DataBar'ın minimum değer nesnesini alır. Buna null veya FormatConditionValueType.Max tipinde CFValueObject atanamaz.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


Veri çubuğunun minimum uzunluğunu temsil eder.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


Bir veri çubuğu koşullu biçimlendirme kuralı ile ilişkili NegativeBarFormat nesnesini alır.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı alır. Varsayılan değer doğrudur.

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


Koşullu biçimlendirmeye sahip hücreler için eksenin rengini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının eksen konumunu ayarlar.

Bakınız [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


Bir veri çubuğunun renk ile nasıl doldurulacağını ayarlar.

Bakınız [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Bu DataBar'ın Rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


Veri çubuğunun görüntülendiği yönü ayarlar.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Veri çubuğunun maksimum uzunluğunu temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


Veri çubuğunun minimum uzunluğunu temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı ayarlar. Varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


Hücredeki veri çubuğunu görüntü bayt dizisine render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Veri çubuğunun hangi hücrede görüntüleneceğini belirtin. |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions, çıktı görüntüsünün bazı özelliklerini içerir. |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

