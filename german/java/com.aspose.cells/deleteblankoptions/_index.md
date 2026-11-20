---
title: "DeleteBlankOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Einstellung zum Löschen leerer Zellen/Zeilen/Spalten dar."
type: docs
url: /de/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

Stellt die Einstellung zum Löschen leerer Zellen/Zeilen/Spalten dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm... als leer betrachtet werden. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder eine leere Zeichenfolge ist. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert eine leere Zeichenfolge ist. |
| [getEndIndex()](#getEndIndex--) | Gibt den Endzeilen-/Spaltenindex (einschließlich) des Bereichs an, der überprüft und leere Zeilen/Spalten gelöscht werden sollen. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Ermittelt den Monitor zum Verfolgen von Änderungen, die durch das Löschen verursacht werden. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden. |
| [getStartIndex()](#getStartIndex--) | Gibt den Startzeilen-/Spaltenindex des zu prüfenden Bereichs an, um leere Zeilen/Spalten zu löschen. |
| [getUpdateReference()](#getUpdateReference--) | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm... als leer betrachtet werden. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder eine leere Zeichenfolge ist. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert eine leere Zeichenfolge ist. |
| [setEndIndex(int value)](#setEndIndex-int-) | Gibt den Endzeilen-/Spaltenindex (einschließlich) des Bereichs an, der überprüft und leere Zeilen/Spalten gelöscht werden sollen. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Legt den Monitor zum Verfolgen von Änderungen fest, die durch das Löschen verursacht werden. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden. |
| [setStartIndex(int value)](#setStartIndex-int-) | Gibt den Startzeilen-/Spaltenindex des zu prüfenden Bereichs an, um leere Zeilen/Spalten zu löschen. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm... als leer betrachtet werden. Der Standardwert ist true.

**Remarks**

Wenn diese Eigenschaft auf false gesetzt wird, werden alle von Zeichenobjekten bedeckten Zeilen/Spalten nicht als leer betrachtet und nicht gelöscht.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


Ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder ein leerer String ist. Der Standardwert ist false.

**Remarks**

Im Allgemeinen sollte der Benutzer sicherstellen, dass die Formeln berechnet wurden, bevor ein Löschvorgang mit dieser Eigenschaft auf true durchgeführt wird. Andernfalls werden alle neu erstellten Formeln über normale APIs wie [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) als leer betrachtet und können gelöscht werden, da ihre berechneten Ergebnisse vor der Berechnung alle null sind.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert ein leerer String ist. Der Standardwert ist true.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


Gibt den Endzeilen-/Spaltenindex (inklusive) des zu prüfenden Bereichs an, um leere Zeilen/Spalten zu löschen. Der Standardwert ist -1, wobei -1 den maximalen Bereich aller zu prüfenden Objekte (Zellen, Zeichnungen, ...) bedeutet.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


Ermittelt den Monitor zum Verfolgen von Änderungen, die durch das Löschen verursacht werden.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden.

Siehe [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Für [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) werden alle Zellen darin als leer betrachtet, außer der nicht-leeren oberen linken Zelle. Dies ist der Standardwert dieser Eigenschaft.

Für [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) werden alle Zellen darin als nicht leer betrachtet.

Für [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) werden alle Zellen außerhalb des Anzeigebereichs des Inhalts als leer betrachtet.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Gibt den Startzeilen-/Spaltenindex des zu prüfenden Bereichs an, um leere Zeilen/Spalten zu löschen.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.

**Remarks**

Ab Version 26.7 setzen wir den Standardwert dieser Eigenschaft auf true.

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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm... als leer betrachtet werden. Der Standardwert ist true.

**Remarks**

Wenn diese Eigenschaft auf false gesetzt wird, werden alle von Zeichenobjekten bedeckten Zeilen/Spalten nicht als leer betrachtet und nicht gelöscht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


Ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder ein leerer String ist. Der Standardwert ist false.

**Remarks**

Im Allgemeinen sollte der Benutzer sicherstellen, dass die Formeln berechnet wurden, bevor ein Löschvorgang mit dieser Eigenschaft auf true durchgeführt wird. Andernfalls werden alle neu erstellten Formeln über normale APIs wie [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) als leer betrachtet und können gelöscht werden, da ihre berechneten Ergebnisse vor der Berechnung alle null sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert ein leerer String ist. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


Gibt den Endzeilen-/Spaltenindex (inklusive) des zu prüfenden Bereichs an, um leere Zeilen/Spalten zu löschen. Der Standardwert ist -1, wobei -1 den maximalen Bereich aller zu prüfenden Objekte (Zellen, Zeichnungen, ...) bedeutet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


Legt den Monitor zum Verfolgen von Änderungen fest, die durch das Löschen verursacht werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden.

Siehe [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Für [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) werden alle Zellen darin als leer betrachtet, außer der nicht-leeren oberen linken Zelle. Dies ist der Standardwert dieser Eigenschaft.

Für [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) werden alle Zellen darin als nicht leer betrachtet.

Für [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) werden alle Zellen außerhalb des Anzeigebereichs des Inhalts als leer betrachtet.



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


Gibt den Startzeilen-/Spaltenindex des zu prüfenden Bereichs an, um leere Zeilen/Spalten zu löschen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.

**Remarks**

Ab Version 26.7 setzen wir den Standardwert dieser Eigenschaft auf true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

