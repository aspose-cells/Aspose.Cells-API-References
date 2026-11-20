---
title: "DataBar"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Beschreibt die DataBar‑Bedingte‑Formatierungsregel."
type: docs
url: /de/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

Beschreiben Sie die DataBar-Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel zeigt einen abgestuften Datenbalken im Zellbereich an.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | Ermittelt die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken. |
| [getAxisPosition()](#getAxisPosition--) | Ermittelt die Position der Achse der Datenbalken, die durch eine bedingte Formatierungsregel festgelegt ist. |
| [getBarBorder()](#getBarBorder--) | Ermittelt ein Objekt, das den Rand eines Datenbalkens festlegt. |
| [getBarFillType()](#getBarFillType--) | Ermittelt, wie ein Datenbalken mit Farbe gefüllt wird. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Ermittelt die Farbe dieses DataBar. |
| [getDirection()](#getDirection--) | Ermittelt die Richtung, in der der Datenbalken angezeigt wird. |
| [getMaxCfvo()](#getMaxCfvo--) | Ermittelt das Maximalwertobjekt dieses DataBar. |
| [getMaxLength()](#getMaxLength--) | Stellt die maximale Länge des Datenbalkens dar. |
| [getMinCfvo()](#getMinCfvo--) | Ermittelt das Minimalwertobjekt dieses DataBar. |
| [getMinLength()](#getMinLength--) | Stellt die minimale Länge des Datenbalkens dar. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Ermittelt das NegativeBarFormat-Objekt, das mit einer Datenbalken‑Bedingten-Formatierungsregel verknüpft ist. |
| [getShowValue()](#getShowValue--) | Ermittelt das Flag, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Ermittelt die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Legt die Position der Achse der Datenbalken fest, die durch eine bedingte Formatierungsregel definiert sind. |
| [setBarFillType(int value)](#setBarFillType-int-) | Legt fest, wie ein Datenbalken mit Farbe gefüllt wird. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Legt die Farbe dieses DataBar fest. |
| [setDirection(int value)](#setDirection-int-) | Legt die Richtung fest, in der der Datenbalken angezeigt wird. |
| [setMaxLength(int value)](#setMaxLength-int-) | Stellt die maximale Länge des Datenbalkens dar. |
| [setMinLength(int value)](#setMinLength-int-) | Stellt die minimale Länge des Datenbalkens dar. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Legt das Flag fest, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Rendert den Datenbalken in einer Zelle zu einem Bild‑Byte‑Array. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


Ermittelt die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


Ermittelt die Position der Achse der Datenbalken, die durch eine bedingte Formatierungsregel festgelegt ist.

Siehe [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


Ermittelt ein Objekt, das den Rand eines Datenbalkens festlegt.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


Ermittelt, wie ein Datenbalken mit Farbe gefüllt wird.

Siehe [DataBarFillType](../../com.aspose.cells/databarfilltype).

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


Ermittelt die Farbe dieses DataBar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


Ermittelt die Richtung, in der der Datenbalken angezeigt wird.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Ermittelt das Maximalwertobjekt dieses DataBar. Es kann nicht null oder ein CFValueObject vom Typ FormatConditionValueType.Min zugewiesen werden.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Stellt die maximale Länge des Datenbalkens dar.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Ermittelt das Minimalwertobjekt dieses DataBar. Es kann nicht null oder ein CFValueObject vom Typ FormatConditionValueType.Max zugewiesen werden.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


Stellt die minimale Länge des Datenbalkens dar.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


Ermittelt das NegativeBarFormat-Objekt, das mit einer Datenbalken‑Bedingten-Formatierungsregel verknüpft ist.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Ermittelt das Flag, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. Der Standardwert ist true.

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


Ermittelt die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


Legt die Position der Achse der Datenbalken fest, die durch eine bedingte Formatierungsregel definiert sind.

Siehe [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


Legt fest, wie ein Datenbalken mit Farbe gefüllt wird.

Siehe [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Legt die Farbe dieses DataBar fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


Legt die Richtung fest, in der der Datenbalken angezeigt wird.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Stellt die maximale Länge des Datenbalkens dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


Stellt die minimale Länge des Datenbalkens dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Legt das Flag fest, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


Rendert den Datenbalken in einer Zelle zu einem Bild‑Byte‑Array.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Geben Sie an, in welcher Zelle der Datenbalken gerendert werden soll |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions enthält einige Eigenschaften des Ausgabebildes |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

