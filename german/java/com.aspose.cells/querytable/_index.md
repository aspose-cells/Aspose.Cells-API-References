---
title: "QueryTable"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt QueryTable-Informationen dar."
type: docs
url: /de/java/com.aspose.cells/querytable/
---

**Inheritance:**
java.lang.Object
```
public class QueryTable
```

Stellt QueryTable-Informationen dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Getting the first query table in the worksheet if exists
         //QueryTable qt = worksheet.QueryTables[0];
         //Getting display address of the query table.
         //string address = qt.ResultRange.Address;
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdjustColumnWidth()](#getAdjustColumnWidth--) | Gibt die AdjustColumnWidth des Objekts zurück oder setzt sie. |
| [getClass()](#getClass--) |  |
| [getConnectionId()](#getConnectionId--) | Ermittelt die Verbindungs-ID der Abfrage-Tabelle. |
| [getExternalConnection()](#getExternalConnection--) | Ermittelt die zugehörige externe Verbindung. |
| [getName()](#getName--) | Liefert den Namen der querytable. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Gibt den PreserveFormatting des Objekts zurück oder setzt ihn. |
| [getResultRange()](#getResultRange--) | Liefert den Bereich des Ergebnisses. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdjustColumnWidth(boolean value)](#setAdjustColumnWidth-boolean-) | Gibt die AdjustColumnWidth des Objekts zurück oder setzt sie. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Gibt den PreserveFormatting des Objekts zurück oder setzt ihn. |
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
### getAdjustColumnWidth() {#getAdjustColumnWidth--}
```
public boolean getAdjustColumnWidth()
```


Gibt die AdjustColumnWidth des Objekts zurück oder setzt sie.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Ermittelt die Verbindungs-ID der Abfrage-Tabelle.

**Returns:**
int
### getExternalConnection() {#getExternalConnection--}
```
public ExternalConnection getExternalConnection()
```


Ermittelt die zugehörige externe Verbindung.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen der querytable.

**Returns:**
java.lang.String
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Gibt den PreserveFormatting des Objekts zurück oder setzt ihn.

**Returns:**
boolean
### getResultRange() {#getResultRange--}
```
public Range getResultRange()
```


Liefert den Bereich des Ergebnisses.

**Returns:**
[Range](../../com.aspose.cells/range) - 
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




### setAdjustColumnWidth(boolean value) {#setAdjustColumnWidth-boolean-}
```
public void setAdjustColumnWidth(boolean value)
```


Gibt die AdjustColumnWidth des Objekts zurück oder setzt sie.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Gibt den PreserveFormatting des Objekts zurück oder setzt ihn.

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

