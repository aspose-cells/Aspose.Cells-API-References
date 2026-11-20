---
title: "GridWorksheetCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

Kapselt eine Sammlung von [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add()](#add--) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String sheetName)](#add-java.lang.String-) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [calculateFormula()](#calculateFormula--) | Berechnet das Ergebnis von Formeln. |
| [clear()](#clear--) | Alle Arbeitsblätter löschen. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-Element am angegebenen Index. |
| [get(String sheetName)](#get-java.lang.String-) | Liefert das [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-Element mit dem angegebenen Namen. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Größe des Enumerators ab. |
| [getDefaultFontName()](#getDefaultFontName--) | Liefert den Standard-Schriftartnamen der Steuerung. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Ermittelt die Sammlung aller Name-Objekte im Tabellenblatt. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Ermittelt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Fügt ein Arbeitsblatt ein. |
| [iterator()](#iterator--) | Ruft den Zeilen-Enumerator ab. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element an einem angegebenen Index. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Entfernt das Element mit einem angegebenen Namen. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Legt den Standard‑Schriftartnamen des Steuerelements fest. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Legt das Dezimaltrennzeichen für das Formatieren/Parsen numerischer Werte fest. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Legt die Sichtbarkeit für das Blatt fest. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Vertauscht die beiden Blätter. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Fügt der Sammlung ein Arbeitsblatt hinzu.

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) Objektindex.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


Fügt der Sammlung ein Arbeitsblatt hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Arbeitsblattname |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Index des Quellarbeitsblatts. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) Objektindex.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Name des Quellarbeitsblatts. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) Objektindex.
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Berechnet das Ergebnis von Formeln.

### clear() {#clear--}
```
public void clear()
```


Alle Arbeitsblätter löschen.

**Remarks**

Ein Arbeitsbuch muss ein Arbeitsblatt enthalten.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
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
public GridWorksheet get(int index)
```


Liefert das [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


Liefert das [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-Element mit dem angegebenen Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Der Name des Arbeitsblatts. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

**Remarks**

Der Arbeitsblattindex ist nullbasiert.

**Returns:**
int
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


Ruft die Größe des Enumerators ab.

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Liefert den Standard-Schriftartnamen der Steuerung.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


Ermittelt die Sammlung aller Name-Objekte im Tabellenblatt.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Liest das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte. Standard ist das Dezimaltrennzeichen der aktuellen Region.

**Returns:**
char
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


Fügt ein Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Blattindex |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ruft den Zeilen-Enumerator ab.

**Returns:**
java.util.Iterator – Der Zeilen-Enumerator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt das Element an einem angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Indexwert des zu entfernenden Elements. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Entfernt das Element mit einem angegebenen Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des zu entfernenden Elements. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

**Remarks**

Der Arbeitsblattindex ist nullbasiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Legt den Standard‑Schriftartnamen des Steuerelements fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Legt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte fest. Standard ist das Dezimaltrennzeichen der aktuellen Region.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


Legt die Sichtbarkeit für das Blatt fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Name des Quellarbeitsblatts. |
| isVisible | boolean | Ob das Arbeitsblatt sichtbar ist |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Vertauscht die beiden Blätter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex1 | int | Das erste Arbeitsblatt. |
| sheetIndex2 | int | Das zweite Arbeitsblatt. |

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

