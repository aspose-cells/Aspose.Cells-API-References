---
title: "DataBar"
second_title: "Aspose.Cells för Java API-referens"
description: "Beskriv DataBar‑villkorsformatregeln."
type: docs
url: /sv/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

Beskriv DataBar conditional formatting rule. Denna villkorsformatregel visar en graderad datastapel i cellintervallet.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | Hämtar färgen på axeln för celler med villkorsformat som datastaplar. |
| [getAxisPosition()](#getAxisPosition--) | Hämtar positionen för axeln på datastaplarna som specificeras av en villkorsformatregel. |
| [getBarBorder()](#getBarBorder--) | Hämtar ett objekt som specificerar kanten på en datastapel. |
| [getBarFillType()](#getBarFillType--) | Hämtar hur en datastapel fylls med färg. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Hämtar den här DataBar's Color. |
| [getDirection()](#getDirection--) | Hämtar riktningen som databar är visad. |
| [getMaxCfvo()](#getMaxCfvo--) | Hämtar detta DataBar's max value object. |
| [getMaxLength()](#getMaxLength--) | Representerar den maximala längden på datafältet. |
| [getMinCfvo()](#getMinCfvo--) | Hämtar detta DataBar:s minsta värdeobjekt. |
| [getMinLength()](#getMinLength--) | Representerar den minsta längden på datafältet. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Hämtar NegativeBarFormat-objektet som är associerat med en villkorsstyrd formateringsregel för datafält. |
| [getShowValue()](#getShowValue--) | Hämtar flaggan som indikerar om värdena i cellerna som detta datafält tillämpas på ska visas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Hämtar färgen på axeln för celler med villkorsformat som datastaplar. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Ställer in positionen för axeln på datafälten som specificeras av en villkorsstyrd formateringsregel. |
| [setBarFillType(int value)](#setBarFillType-int-) | Ställer in hur ett datafält fylls med färg. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Ställer in detta DataBar:s färg. |
| [setDirection(int value)](#setDirection-int-) | Ställer in riktningen som datafältet visas i. |
| [setMaxLength(int value)](#setMaxLength-int-) | Representerar den maximala längden på datafältet. |
| [setMinLength(int value)](#setMinLength-int-) | Representerar den minsta längden på datafältet. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Ställer in flaggan som indikerar om värdena i cellerna som detta datafält tillämpas på ska visas. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Rendera datafält i cell till bildens byte-array. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


Hämtar färgen på axeln för celler med villkorsformat som datastaplar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


Hämtar positionen för axeln på datastaplarna som specificeras av en villkorsformatregel.

Se [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


Hämtar ett objekt som specificerar kanten på en datastapel.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


Hämtar hur en datastapel fylls med färg.

Se [DataBarFillType](../../com.aspose.cells/databarfilltype).

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


Hämtar den här DataBar's Color.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


Hämtar riktningen som databar är visad.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Hämtar detta DataBar:s maxvärdeobjekt. Kan inte sätta null eller CFValueObject med typen FormatConditionValueType.Min till det.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Representerar den maximala längden på datafältet.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Hämtar detta DataBar:s minvärdeobjekt. Kan inte sätta null eller CFValueObject med typen FormatConditionValueType.Max till det.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


Representerar den minsta längden på datafältet.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


Hämtar NegativeBarFormat-objektet som är associerat med en villkorsstyrd formateringsregel för datafält.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Hämtar flaggan som indikerar om värdena i cellerna som detta datafält tillämpas på ska visas. Standardvärdet är true.

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


Hämtar färgen på axeln för celler med villkorsformat som datastaplar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


Ställer in positionen för axeln på datafälten som specificeras av en villkorsstyrd formateringsregel.

Se [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


Ställer in hur ett datafält fylls med färg.

Se [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Ställer in detta DataBar:s färg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


Ställer in riktningen som datafältet visas i.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Representerar den maximala längden på datafältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


Representerar den minsta längden på datafältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Ställer in flaggan som indikerar om värdena i cellerna som detta datafält tillämpas på ska visas. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


Rendera datafält i cell till bildens byte-array.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Anger i vilken cell datafältet ska renderas |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions innehåller vissa egenskaper för utdata bilden |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

