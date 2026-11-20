---
title: "FormatConditionCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die bedingte Formatierung dar."
type: docs
url: /de/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

Stellt die bedingte Formatierung dar. Die FormatConditions können bis zu drei bedingte Formate enthalten.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         //Saving the Excel file
         workbook.save("output.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Fügt eine Formatierungsbedingung und den betroffenen Zellbereich zu den FormatConditions hinzu. Die FormatConditions können bis zu drei bedingte Formate enthalten. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Fügt einen bedingt formatierten Zellbereich hinzu. |
| [addCondition(int type)](#addCondition-int-) | Füge eine Formatbedingung hinzu. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Fügt eine Formatierungsbedingung hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gibt die Formatierungsbedingung nach Index zurück. |
| [getCellArea(int index)](#getCellArea-int-) | Liefert den bedingt formatierten Zellbereich nach Index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Liefert die Anzahl der Bedingungen. |
| [getRangeCount()](#getRangeCount--) | Liefert die Anzahl der bedingt formatierten Bereiche. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Entfernt den bedingt formatierten Zellbereich nach Index. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Entfernt die bedingte Formatierung im Bereich. |
| [removeCondition(int index)](#removeCondition-int-) | Entfernt die Formatierungsbedingung nach Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


Fügt eine Formatierungsbedingung und den betroffenen Zellbereich zu den FormatConditions hinzu. Die FormatConditions können bis zu drei bedingte Formate enthalten. Verweise auf andere Tabellenblätter sind in den Formeln der bedingten Formatierung nicht zulässig.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Bedingt formatierter Zellbereich. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Typ der bedingten Formatierung. Es könnte eines der Mitglieder von FormatConditionType sein. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Vergleichsoperator. Es könnte eines der Mitglieder von OperatorType sein. |
| formula1 | java.lang.String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| formula2 | java.lang.String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist |

**Returns:**
int[] - [0]:Index des Formatierungsbedingungen-Objekts;[1] Index des betroffenen Zellbereichs.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


Fügt einen bedingt formatierten Zellbereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Bedingt formatierter Zellbereich. |

**Returns:**
int - Index des bedingt formatierten Zellbereichs.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


Füge eine Formatbedingung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Formatbedingungstyp. |

**Returns:**
int - Index des Formatierungsbedingungen-Objekts;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


Fügt eine Formatierungsbedingung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Der Typ der Formatbedingung. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Der Operator-Typ |
| formula1 | java.lang.String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. Wenn der Eingabewert mit '=', beginnt, wird er als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=', beginnen, kann der Benutzer sie im Format "=\\"=...\\"" als Formel eingeben. |
| formula2 | java.lang.String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. Das Eingabeformat ist dasselbe wie bei formula1. |

**Returns:**
int - Index des Formatierungsbedingungen-Objekts;
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```


Gibt die Formatierungsbedingung nach Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | der Index der zurückzugebenden Formatierungsbedingung. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


Liefert den bedingt formatierten Zellbereich nach Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | der Index des bedingt formatierten Zellbereichs. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Liefert die Anzahl der Bedingungen.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Liefert die Anzahl der bedingt formatierten Bereiche.

**Returns:**
int
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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


Entfernt den bedingt formatierten Zellbereich nach Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des zu entfernenden bedingt formatierten Zellbereichs. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Entfernt die bedingte Formatierung im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die startRow des Bereichs. |
| startColumn | int | Die startColumn des Bereichs. |
| totalRows | int | Die Anzahl der Zeilen des Bereichs. |
| totalColumns | int | Die Anzahl der Spalten des Bereichs. |

**Returns:**
boolean - Gibt TRUE zurück, diese FormatCondtionCollection sollte entfernt werden.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


Entfernt die Formatierungsbedingung nach Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index der zu entfernenden Formatierungsbedingung. |

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

