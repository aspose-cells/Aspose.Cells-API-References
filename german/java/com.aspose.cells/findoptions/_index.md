---
title: "FindOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt Suchoptionen dar."
type: docs
url: /de/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Stellt Suchoptionen dar.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Gibt an, ob die gesuchte Zeichenfolge groß‑/kleinschreibungssensitiv ist. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Ermittelt einen Wert, der angibt, ob der gesuchte Zeichenfolgenwert in numerische Daten konvertiert wird. |
| [getLookAtType()](#getLookAtType--) | Typ ansehen. |
| [getLookInType()](#getLookInType--) | Im Typ nachsehen. |
| [getRange()](#getRange--) | Liest und setzt den gesuchten Bereich. |
| [getRegexKey()](#getRegexKey--) | Gibt an, ob der gesuchte Schlüssel ein regulärer Ausdruck ist. |
| [getSearchBackward()](#getSearchBackward--) | Ob rückwärts nach Zellen gesucht wird. |
| [getSearchNext()](#getSearchNext--) | Suchreihenfolge. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt. |
| [getStyle()](#getStyle--) | Das zu suchende Format. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Gibt an, ob der Typ des gesuchten Zellwerts mit dem gesuchten Schlüssel übereinstimmen soll. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Gibt an, ob der gesuchte Bereich festgelegt ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Gibt an, ob die gesuchte Zeichenfolge groß‑/kleinschreibungssensitiv ist. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Legt einen Wert fest, der angibt, ob der gesuchte Zeichenfolgenwert in numerische Daten konvertiert werden soll. |
| [setLookAtType(int value)](#setLookAtType-int-) | Typ ansehen. |
| [setLookInType(int value)](#setLookInType-int-) | Im Typ nachsehen. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Legt den gesuchten Bereich fest. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Gibt an, ob der gesuchte Schlüssel ein regulärer Ausdruck ist. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Ob rückwärts nach Zellen gesucht wird. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Suchreihenfolge. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Das zu suchende Format. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Gibt an, ob der Typ des gesuchten Zellwerts mit dem gesuchten Schlüssel übereinstimmen soll. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Gibt an, ob die gesuchte Zeichenfolge groß‑/kleinschreibungssensitiv ist.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Ermittelt einen Wert, der angibt, ob der gesuchte Zeichenfolgenwert in numerische Daten konvertiert wird.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Typ ansehen.

Siehe [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Wenn [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) true ist und der Benutzer die genaue Regel für das Regex angegeben hat, sollte aus Leistungsgründen diese Eigenschaft als [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) festgelegt werden. Andernfalls werden wir den Suchschlüssel umgestalten, um sicherzustellen, dass er gemäß dem jeweiligen Typ übereinstimmen kann. Zum Beispiel, wenn der Typ [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) ist (dies ist der Standardwert für diese Eigenschaft), fügen wir automatisch Platzhalter am Anfang und Ende des Suchschlüssels hinzu. In diesem Fall werden die regulären Ausdrücke komplexer und die Leistung wird ebenfalls sinken.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


Im Typ nachsehen.

Siehe [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


Liest und setzt den gesuchten Bereich.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex genommen und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst.

**Remarks**

Obwohl der Suchschlüssel als Regex angegeben wurde, kann er gemäß dem angegebenen [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) umgestaltet werden. Zum Beispiel, wenn der Typ [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) ist (dies ist der Standardwert für diese Optionen), werden automatisch Platzhalter am Anfang und Ende des Suchschlüssels hinzugefügt, um sicherzustellen, dass die Übereinstimmung als „contains“ geprüft wird. In diesem Fall werden die regulären Ausdrücke komplexer und die Leistung wird ebenfalls sinken. Daher, aus Leistungsgründen, wenn der Benutzer die genaue Regel für das Regex angegeben hat, ist es nicht nötig, [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) als zusätzliche Einschränkung zu verwenden, und der Benutzer kann es als [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) festlegen, um bessere Leistung zu erzielen.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


Ob rückwärts nach Zellen gesucht wird.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


Suchreihenfolge. True: nächstes Element suchen. False: vorheriges Element suchen.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft FindOptions.SearchBackward. Diese Eigenschaft wird 12 Monate später, seit November 2018, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Das zu suchende Format.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


Gibt an, ob der Typ des gesuchten Zellwerts mit dem gesuchten Schlüssel übereinstimmen soll.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


Gibt an, ob der gesuchte Bereich festgelegt ist.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Gibt an, ob die gesuchte Zeichenfolge groß‑/kleinschreibungssensitiv ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Legt einen Wert fest, der angibt, ob der gesuchte Zeichenfolgenwert in numerische Daten konvertiert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


Typ ansehen.

Siehe [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Wenn [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) true ist und der Benutzer die genaue Regel für das Regex angegeben hat, sollte aus Leistungsgründen diese Eigenschaft als [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) festgelegt werden. Andernfalls werden wir den Suchschlüssel umgestalten, um sicherzustellen, dass er gemäß dem jeweiligen Typ übereinstimmen kann. Zum Beispiel, wenn der Typ [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) ist (dies ist der Standardwert für diese Eigenschaft), fügen wir automatisch Platzhalter am Anfang und Ende des Suchschlüssels hinzu. In diesem Fall werden die regulären Ausdrücke komplexer und die Leistung wird ebenfalls sinken.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


Im Typ nachsehen.

Siehe [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


Legt den gesuchten Bereich fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | der gesuchte Bereich. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex genommen und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst.

**Remarks**

Obwohl der Suchschlüssel als Regex angegeben wurde, kann er gemäß dem angegebenen [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) umgestaltet werden. Zum Beispiel, wenn der Typ [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) ist (dies ist der Standardwert für diese Optionen), werden automatisch Platzhalter am Anfang und Ende des Suchschlüssels hinzugefügt, um sicherzustellen, dass die Übereinstimmung als „contains“ geprüft wird. In diesem Fall werden die regulären Ausdrücke komplexer und die Leistung wird ebenfalls sinken. Daher, aus Leistungsgründen, wenn der Benutzer die genaue Regel für das Regex angegeben hat, ist es nicht nötig, [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) als zusätzliche Einschränkung zu verwenden, und der Benutzer kann es als [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) festlegen, um bessere Leistung zu erzielen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


Ob rückwärts nach Zellen gesucht wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


Suchreihenfolge. True: nächstes Element suchen. False: vorheriges Element suchen.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft FindOptions.SearchBackward. Diese Eigenschaft wird 12 Monate später, seit November 2018, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Das zu suchende Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


Gibt an, ob der Typ des gesuchten Zellwerts mit dem gesuchten Schlüssel übereinstimmen soll.

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

