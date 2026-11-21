---
title: "ListColumn"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en kolumn i en tabell."
type: docs
url: /sv/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

Representerar en kolumn i en tabell.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Hämtar formeln för den här listkolumnen. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Hämtar formeln för totalsraden i den här listkolumnen. |
| [getDataStyle()](#getDataStyle--) | Hämtar stilen för data i den här kolumnen i tabellen. |
| [getFormula()](#getFormula--) | Hämtar formeln för listkolumnen. |
| [getName()](#getName--) | Hämtar namnet på kolumnen. |
| [getRange()](#getRange--) | Hämtar intervallet för den här listkolumnen. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Hämtar typen av beräkning i totalsraden för listkolumnen. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Hämtar visningsetiketterna för totalsraden. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Indikerar om formeln är en matrisformel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Ställer in formeln för den här listkolumnen. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Hämtar formeln för totalsraden i den här listkolumnen. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Ställer in stilen för data i den här kolumnen i tabellen. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Ställer in formeln för listkolumnen. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på kolumnen. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Ställer in typen av beräkning i totalsraden för listkolumnen. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Ställer in visningsetiketterna för totalsraden. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


Hämtar formeln för den här listkolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Formeln för den här listkolumnen.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


Hämtar formeln för totalsraden i den här listkolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Formeln för den här listkolumnen.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


Hämtar stilen för data i den här kolumnen i tabellen.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Hämtar formeln för listkolumnen.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på kolumnen.

**Remarks**

Om namnet på kolumnen sätts, kommer det motsvarande cellvärdet också att ändras.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Hämtar intervallet för den här listkolumnen.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


Hämtar typen av beräkning i totalsraden för listkolumnen.

Se [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


Hämtar visningsetiketterna för totalsraden.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Indikerar om formeln är en matrisformel.

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




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


Ställer in formeln för den här listkolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | formeln för den här listkolumnen. |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


Hämtar formeln för totalsraden i den här listkolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | formeln för den här listkolumnen. |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


Ställer in stilen för data i den här kolumnen i tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Ställer in formeln för listkolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på kolumnen.

**Remarks**

Om namnet på kolumnen sätts, kommer det motsvarande cellvärdet också att ändras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


Ställer in typen av beräkning i totalsraden för listkolumnen.

Se [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


Ställer in visningsetiketterna för totalsraden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

