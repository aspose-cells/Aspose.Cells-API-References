---
title: "Name"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen definierten Namen für einen Zellenbereich dar."
type: docs
url: /de/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

Stellt einen definierten Namen für einen Zellenbereich dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Ruft den Kommentar des Namens ab. |
| [getFullText()](#getFullText--) | Ruft den vollständigen Text des Namens des Objekts mit der Geltungsbereichseinstellung ab. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | Ruft eine R1C1‑Referenz des [Name](../../com.aspose.cells/name) ab. |
| [getRange()](#getRange--) | Ruft den Bereich ab, wenn dieser Name auf einen Bereich verweist. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Ruft den Bereich ab, wenn dieser Name auf einen Bereich verweist |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Ruft den Bereich ab, wenn dieser Name auf einen Bereich verweist. |
| [getRanges()](#getRanges--) | Ruft alle Bereiche ab, auf die dieser Name verweist. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Ruft alle Bereiche ab, auf die dieser Name verweist. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Ruft alle Referenzen ab, auf die dieser Name verweist. |
| [getRefersTo()](#getRefersTo--) | Gibt die Formel zurück oder legt sie fest, auf die der Name definiert ist, beginnend mit einem Gleichheitszeichen. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Rufe die Referenz dieses Namens ab. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Rufe die Referenz dieses Namens basierend auf der angegebenen Zelle ab. |
| [getSheetIndex()](#getSheetIndex--) | Gibt an, ob dieser Name zu einer Arbeitsmappe oder einem Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert). |
| [getText()](#getText--) | Ruft den Namens-Text des Objekts ab. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Gibt an, ob dieser Name von anderen Formeln referenziert wird. |
| [isVisible()](#isVisible--) | Gibt an, ob der Name sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Setzt den Kommentar des Namens. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | Setzt eine R1C1-Referenz des [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | Gibt die Formel zurück oder legt sie fest, auf die der Name definiert ist, beginnend mit einem Gleichheitszeichen. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Setzt die Referenz dieses Namens. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Gibt an, ob dieser Name zu einer Arbeitsmappe oder einem Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert). |
| [setText(String value)](#setText-java.lang.String-) | Ruft den Namens-Text des Objekts ab. |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob der Name sichtbar ist. |
| [toString()](#toString--) | Gibt einen String zurück, der das aktuelle Range-Objekt darstellt. |
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
### getComment() {#getComment--}
```
public String getComment()
```


Liest den Kommentar des Namens. Gilt nur für Excel 2007 oder höhere Versionen.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


Ruft den vollständigen Text des Namens des Objekts mit der Geltungsbereichseinstellung ab.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


Ruft eine R1C1‑Referenz des [Name](../../com.aspose.cells/name) ab.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Ruft den Bereich ab, wenn dieser Name auf einen Bereich verweist.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


Ruft den Bereich ab, wenn dieser Name auf einen Bereich verweist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| neu berechnen | boolean | ob es neu berechnet wird, wenn dieser Name bereits vor diesem Aufruf berechnet wurde. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


Liest den Bereich, wenn sich dieser Name auf einen Bereich bezieht. Ist die Referenz dieses Namens nicht absolut, kann der Bereich für verschiedene Zellen unterschiedlich sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Der entsprechende Blattindex. |
| Zeile | int | Der entsprechende Zeilenindex. |
| Spalte | int | Der entsprechende Spaltenindex |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Ruft alle Bereiche ab, auf die dieser Name verweist.

**Returns:**
com.aspose.cells.Range[] - Alle Bereiche.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


Ruft alle Bereiche ab, auf die dieser Name verweist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| neu berechnen | boolean | ob es neu berechnet wird, wenn dieser Name bereits vor diesem Aufruf berechnet wurde. |

**Returns:**
com.aspose.cells.Range[] - Alle Bereiche.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


Ruft alle Referenzen ab, auf die dieser Name verweist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| neu berechnen | boolean | ob es neu berechnet wird, wenn dieser Name bereits vor diesem Aufruf berechnet wurde. |

**Returns:**
com.aspose.cells.ReferredArea[] - Alle Bereiche.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Gibt die Formel zurück oder legt sie fest, auf die der Name definiert ist, beginnend mit einem Gleichheitszeichen.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


Rufe die Referenz dieses Namens ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Referenz als R1C1 formatiert werden muss. |
| isLocal | boolean | Ob die Referenz nach dem Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


Rufe die Referenz dieses Namens basierend auf der angegebenen Zelle ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Referenz als R1C1 formatiert werden muss. |
| isLocal | boolean | Ob die Referenz nach dem Gebietsschema formatiert werden muss. |
| Zeile | int | Der Zeilenindex der Zelle. |
| Spalte | int | Der Spaltenindex der Zelle. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Gibt an, ob dieser Name zu einer Arbeitsmappe oder einem Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Ruft den Namens-Text des Objekts ab.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Gibt an, ob dieser Name von anderen Formeln referenziert wird.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Gibt an, ob der Name sichtbar ist.

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




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Setzt den Kommentar des Namens. Gilt nur für Excel 2007 oder höhere Versionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


Setzt eine R1C1-Referenz des [Name](../../com.aspose.cells/name).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


Gibt die Formel zurück oder legt sie fest, auf die der Name definiert ist, beginnend mit einem Gleichheitszeichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


Setzt die Referenz dieses Namens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| refersTo | java.lang.String | Die Referenz. |
| isR1C1 | boolean | Ob die Referenz im R1C1-Format vorliegt. |
| isLocal | boolean | Ob die Referenz nach dem Gebietsschema formatiert ist. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Gibt an, ob dieser Name zu einer Arbeitsmappe oder einem Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ruft den Namens-Text des Objekts ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Gibt an, ob der Name sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### toString() {#toString--}
```
public String toString()
```


Gibt einen String zurück, der das aktuelle Range-Objekt darstellt.

**Returns:**
java.lang.String -
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

