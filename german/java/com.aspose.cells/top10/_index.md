---
title: "Top10"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Beschreibt die Top10‑bedingte Formatierungsregel."
type: docs
url: /de/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

Beschreiben Sie die Top10‑Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte im oberen N‑ oder unteren N‑Bereich liegen, wie angegeben.

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
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Top10()](#Top10--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Ermittelt den Wert von "n" in einer "top/bottom n"‑Bedingten-Formatierungsregel. |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Ermittelt, ob eine "top/bottom n"‑Regel eine "bottom n"‑Regel ist. |
| [isPercent()](#isPercent--) | Ermittelt, ob eine "top/bottom n"‑Regel eine "top/bottom n percent"‑Regel ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Legt fest, ob eine "top/bottom n"‑Regel eine "bottom n"‑Regel ist. |
| [setPercent(boolean value)](#setPercent-boolean-) | Legt fest, ob eine "top/bottom n"‑Regel eine "top/bottom n percent"‑Regel ist. |
| [setRank(int value)](#setRank-int-) | Setzt den Wert von "n" in einer "top/bottom n"‑Bedingten-Formatierungsregel. |
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
| Parameter | Typ | Beschreibung |
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


Ermittelt den Wert von "n" in einer "top/bottom n"‑Bedingten-Formatierungsregel. Wenn IsPercent wahr ist, muss der Wert zwischen 0 und 100 liegen. Andernfalls muss er zwischen 0 und 1000 liegen. Der Standardwert ist 10.

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


Ermittelt, ob eine "top/bottom n"‑Regel eine "bottom n"‑Regel ist. Der Standardwert ist false.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Ermittelt, ob eine "top/bottom n"‑Regel eine "top/bottom n percent"‑Regel ist. Der Standardwert ist false.

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


Legt fest, ob eine "top/bottom n"‑Regel eine "bottom n"‑Regel ist. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


Legt fest, ob eine "top/bottom n"‑Regel eine "top/bottom n percent"‑Regel ist. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


Setzt den Wert von "n" in einer "top/bottom n"‑Bedingten-Formatierungsregel. Wenn IsPercent wahr ist, muss der Wert zwischen 0 und 100 liegen. Andernfalls muss er zwischen 0 und 1000 liegen. Der Standardwert ist 10.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

