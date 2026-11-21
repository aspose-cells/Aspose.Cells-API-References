---
title: "CalculationCell"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar den beräkning relevanta data om en cell som beräknas."
type: docs
url: /sv/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

Representerar den beräkning relevanta data om en cell som beräknas.

**Remarks**

Användaren bör inte ändra någon data i Workbook under formelberäkningsprocessen, annars kan oväntade resultat eller undantag uppstå. Så alla objekt som tillhandahålls av denna klass (såsom Cell-objektet för [getCell()](../../com.aspose.cells/calculationcell\#getCell--)) är endast avsedda för \"read\"-ändamål.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Hämtar Cell-objektet som beräknas. |
| [getCellColumn()](#getCellColumn--) | Hämtar kolumnindex för cellen. |
| [getCellRow()](#getCellRow--) | Hämtar radindex för cellen. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Hämtar Workbook-objektet. |
| [getWorksheet()](#getWorksheet--) | Hämtar Worksheet-objektet där cellen finns. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Ställer in det beräknade värdet för cellen. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


Hämtar Cell-objektet som beräknas.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Hämtar kolumnindex för cellen.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Hämtar radindex för cellen.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Hämtar Workbook-objektet.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Hämtar Worksheet-objektet där cellen finns.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


Ställer in det beräknade värdet för cellen.

**Remarks**

Användaren kan sätta det beräknade resultatet med denna metod för att ignorera den automatiska beräkningen för cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| v | java.lang.Object |  |

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

