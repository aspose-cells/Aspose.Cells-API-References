---
title: "UnionRange"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen Union‑Bereich dar."
type: docs
url: /de/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

Stellt einen Union‑Bereich dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet Formate für einen gesamten Bereich an. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Kopieren des Bereichs mit Sonderoptionen für Einfügen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Liefert die Gesamtzahl der Zellen im Bereich. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Gibt die Anzahl der Zeilen im Bereich zurück. |
| [getFirstColumn()](#getFirstColumn--) | Gibt den Index der ersten Spalte des Bereichs zurück. |
| [getFirstRow()](#getFirstRow--) | Gibt den Index der ersten Zeile des Bereichs zurück. |
| [getHyperlinks()](#getHyperlinks--) | Gibt alle Hyperlinks im Bereich zurück. |
| [getName()](#getName--) | Gibt den Namen des Bereichs zurück. |
| [getRangeCount()](#getRangeCount--) | Liefert die Anzahl der Bereiche. |
| [getRanges()](#getRanges--) | Liefert alle Union-Bereiche. |
| [getRefersTo()](#getRefersTo--) | Gibt das 'refers to' des Bereichs zurück. |
| [getRowCount()](#getRowCount--) | Gibt die Anzahl der Zeilen im Bereich zurück. |
| [getValue()](#getValue--) | Liefert die Werte des Bereichs. |
| [hasRange()](#hasRange--) | Gibt an, ob dies einen Bereich hat. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Schneidet einen anderen Bereich. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Schneidet einen anderen Bereich. |
| [intersect(String range)](#intersect-java.lang.String-) | Schneidet einen anderen Bereich. |
| [iterator()](#iterator--) | Gibt den Enumerator für Zellen in diesem Range zurück. |
| [merge()](#merge--) | Kombiniert einen Zellbereich zu einer einzelnen Zelle. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Setzt einen Wert in den Bereich; falls nötig wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [setName(String value)](#setName-java.lang.String-) | Setzt den Namen des Bereichs. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Legt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe fest. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Legt Umrandungsrahmen um einen Zellbereich fest. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Legt den Stil des Bereichs fest. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Setzt die Werte des Bereichs. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Löst zusammengeführte Zellen dieses Bereichs. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Vereint die Bereiche. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Vereint einen anderen Bereich. |
| [union(String range)](#union-java.lang.String-) | Vereint einen anderen Bereich. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Wendet Formate für einen gesamten Bereich an.

**Remarks**

Jede Zelle in diesem Bereich enthält ein [Style](../../com.aspose.cells/style)-Objekt. Daher ist diese Methode speicherintensiv. Bitte verwenden Sie sie vorsichtig.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Das Stilobjekt, das angewendet wird. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags, die angewandte Formatierungseigenschaften anzeigen. |

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


Kopieren des Bereichs mit Sonderoptionen für Einfügen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | Der Quellbereich. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Die Optionen für Einfügen Spezial. |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


Liefert die Gesamtzahl der Zellen im Bereich.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Gibt die Anzahl der Zeilen im Bereich zurück.

**Remarks**

Wirkt nur, wenn es nur einen Bereich enthält.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Gibt den Index der ersten Spalte des Bereichs zurück.

**Remarks**

Wirkt nur, wenn es nur einen Bereich enthält.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Gibt den Index der ersten Zeile des Bereichs zurück.

**Remarks**

Wirkt nur, wenn es nur einen Bereich enthält.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Gibt alle Hyperlinks im Bereich zurück.

**Returns:**
com.aspose.cells.Hyperlink[]
### getName() {#getName--}
```
public String getName()
```


Gibt den Namen des Bereichs zurück.

**Remarks**

Benannte Bereiche werden unterstützt. Zum Beispiel,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Liefert die Anzahl der Bereiche.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Liefert alle Union-Bereiche.

**Returns:**
com.aspose.cells.Range[]
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Gibt das 'refers to' des Bereichs zurück.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Gibt die Anzahl der Zeilen im Bereich zurück.

**Remarks**

Wirkt nur, wenn es nur einen Bereich enthält.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Liefert die Werte des Bereichs.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


Gibt an, ob dies einen Bereich hat.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


Schneidet einen anderen Bereich.

**Remarks**

Wenn die beiden vereinigten Bereiche nicht geschnitten werden, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Der Bereich. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


Schneidet einen anderen Bereich.

**Remarks**

Wenn die beiden vereinigten Bereiche nicht geschnitten werden, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Der Bereich. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


Schneidet einen anderen Bereich.

**Remarks**

Wenn die beiden vereinigten Bereiche nicht geschnitten werden, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | java.lang.String | Der Bereich. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt den Enumerator für Zellen in diesem Range zurück.

**Remarks**

Beim Durchlaufen von Elementen mit dem zurückgegebenen Enumerator sollte die Zellen‑Sammlung nicht verändert werden (z. B. Operationen, die dazu führen, dass neue Cell/Row erzeugt oder vorhandene Cell/Row gelöscht werden). Andernfalls kann der Enumerator möglicherweise nicht alle Zellen korrekt durchlaufen (einige Elemente können mehrfach durchlaufen oder übersprungen werden).

**Returns:**
java.util.Iterator - Der Zellen‑Enumerator
### merge() {#merge--}
```
public void merge()
```


Kombiniert einen Zellbereich zu einer einzelnen Zelle.

**Remarks**

Referenzieren Sie die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich.

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Setzt einen Wert in den Bereich; falls nötig wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert |
| isConverted | boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |
| setStyle | boolean | True: das Zahlenformat auf den Zellenstil setzen, wenn in einen anderen Datentyp konvertiert wird |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Setzt den Namen des Bereichs.

**Remarks**

Benannte Bereiche werden unterstützt. Zum Beispiel,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Legt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Rahmenstil. |
| borderColor | [Color](../../com.aspose.cells/color) | Randfarbe. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Legt Umrandungsrahmen um einen Zellbereich fest.

**Remarks**

Sowohl die Länge von borderStyles als auch von borderStyles muss 4 betragen. Die Reihenfolge von borderStyles und borderStyles muss oben, unten, links, rechts sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Rahmenstile. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Randfarben. |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Legt den Stil des Bereichs fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Das Style-Objekt. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Setzt die Werte des Bereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```


Löst zusammengeführte Zellen dieses Bereichs.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


Vereint die Bereiche.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Die Bereiche. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


Vereint einen anderen Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Der Bereich. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


Vereint einen anderen Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | java.lang.String | Der Bereich. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

