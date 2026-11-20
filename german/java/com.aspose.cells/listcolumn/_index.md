---
title: "ListColumn"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Spalte in einer Tabelle dar."
type: docs
url: /de/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

Stellt eine Spalte in einer Tabelle dar.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Liefert die Formel dieser Listenspalte. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Liefert die Formel der Summenzeile dieser Listenspalte. |
| [getDataStyle()](#getDataStyle--) | Liefert den Stil der Daten in dieser Tabellenspalte. |
| [getFormula()](#getFormula--) | Liefert die Formel der Listenspalte. |
| [getName()](#getName--) | Liefert den Namen der Spalte. |
| [getRange()](#getRange--) | Liefert den Bereich dieser Listenspalte. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Liefert den Berechnungstyp in der Summenzeile der Listenspalte. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Liefert die Anzeige­bezeichnungen der Summenzeile. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Gibt an, ob die Formel eine Array‑Formel ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Setzt die Formel für diese Listenspalte. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Liefert die Formel der Summenzeile dieser Listenspalte. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Setzt den Stil der Daten in dieser Tabellenspalte. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Setzt die Formel der Listenspalte. |
| [setName(String value)](#setName-java.lang.String-) | Setzt den Namen der Spalte. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Setzt den Berechnungstyp in der Summenzeile der Listenspalte. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Setzt die Anzeige­bezeichnungen der Summenzeile. |
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


Liefert die Formel dieser Listenspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Die Formel dieser Listenspalte.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


Liefert die Formel der Summenzeile dieser Listenspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Die Formel dieser Listenspalte.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


Liefert den Stil der Daten in dieser Tabellenspalte.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Liefert die Formel der Listenspalte.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen der Spalte.

**Remarks**

Wenn der Name der Spalte gesetzt wird, wird auch der entsprechende Zellenwert geändert.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Liefert den Bereich dieser Listenspalte.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


Liefert den Berechnungstyp in der Summenzeile der Listenspalte.

Siehe [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


Liefert die Anzeige­bezeichnungen der Summenzeile.

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


Gibt an, ob die Formel eine Array‑Formel ist.

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


Setzt die Formel für diese Listenspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | die Formel für diese Listenspalte. |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


Liefert die Formel der Summenzeile dieser Listenspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | die Formel für diese Listenspalte. |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


Setzt den Stil der Daten in dieser Tabellenspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Setzt die Formel der Listenspalte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Setzt den Namen der Spalte.

**Remarks**

Wenn der Name der Spalte gesetzt wird, wird auch der entsprechende Zellenwert geändert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


Setzt den Berechnungstyp in der Summenzeile der Listenspalte.

Siehe [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


Setzt die Anzeige­bezeichnungen der Summenzeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

