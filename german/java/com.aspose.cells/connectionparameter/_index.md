---
title: "ConnectionParameter"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Gibt Eigenschaften zu allen Parametern an, die mit externen Datenverbindungen verwendet werden. Parameter sind für ODBC- und Webabfragen gültig."
type: docs
url: /de/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Gibt Eigenschaften zu allen Parametern an, die mit externen Datenverbindungen verwendet werden. Parameter sind für ODBC- und Webabfragen gültig.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Der Name des Parameters. |
| [getPrompt()](#getPrompt--) | Eingabeaufforderungszeichenfolge für den Parameter. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Kennzeichen, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert liefert, ändert. |
| [getSqlType()](#getSqlType--) | SQL-Datentyp des Parameters. |
| [getType()](#getType--) | Verwendeter Parametertyp. |
| [getValue()](#getValue--) | Nicht-ganzzahliger numerischer Wert, Ganzzahlwert, Zeichenfolgenwert oder Boolescher Wert, der als Abfrageparameter verwendet wird. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. |
| [setName(String value)](#setName-java.lang.String-) | Der Name des Parameters. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | Eingabeaufforderungszeichenfolge für den Parameter. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | Kennzeichen, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert liefert, ändert. |
| [setSqlType(int value)](#setSqlType-int-) | SQL-Datentyp des Parameters. |
| [setType(int value)](#setType-int-) | Verwendeter Parametertyp. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Nicht-ganzzahliger numerischer Wert, Ganzzahlwert, Zeichenfolgenwert oder Boolescher Wert, der als Abfrageparameter verwendet wird. |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType = cell ist.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Der Name des Parameters.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Eingabeaufforderungszeichenfolge für den Parameter. Wird dem Tabellenbenutzer zusammen mit einer Eingabeoberfläche präsentiert, um den Parameterwert vor dem Aktualisieren der externen Daten zu erfassen. Wird nur verwendet, wenn parameterType = prompt ist.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Kennzeichen, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert liefert, ändert. Wenn true, werden die externen Daten bei jeder Änderung mit dem neuen Parameterwert aktualisiert. Wenn false, werden die externen Daten nur aktualisiert, wenn der Benutzer dies anfordert oder ein anderes Ereignis die Aktualisierung auslöst (z. B. beim Öffnen der Arbeitsmappe).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


SQL-Datentyp des Parameters. Nur gültig für ODBC-Quellen.

Siehe [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Verwendeter Parametertyp. Wenn parameterType=value, wird der Wert aus boolean, double, integer oder string verwendet. In diesem Fall wird erwartet, dass nur einer der \{boolean, double, integer oder string\} angegeben wird.

Siehe [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Nicht-ganzzahliger numerischer Wert, Ganzzahlwert, Zeichenfolgenwert oder Boolescher Wert, der als Abfrageparameter verwendet wird. Wird nur verwendet, wenn parameterType = value ist.

**Returns:**
java.lang.Object
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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType = cell ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Der Name des Parameters.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


Eingabeaufforderungszeichenfolge für den Parameter. Wird dem Tabellenbenutzer zusammen mit einer Eingabeoberfläche präsentiert, um den Parameterwert vor dem Aktualisieren der externen Daten zu erfassen. Wird nur verwendet, wenn parameterType = prompt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


Kennzeichen, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert liefert, ändert. Wenn true, werden die externen Daten bei jeder Änderung mit dem neuen Parameterwert aktualisiert. Wenn false, werden die externen Daten nur aktualisiert, wenn der Benutzer dies anfordert oder ein anderes Ereignis die Aktualisierung auslöst (z. B. beim Öffnen der Arbeitsmappe).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


SQL-Datentyp des Parameters. Nur gültig für ODBC-Quellen.

Siehe [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Verwendeter Parametertyp. Wenn parameterType=value, wird der Wert aus boolean, double, integer oder string verwendet. In diesem Fall wird erwartet, dass nur einer der \{boolean, double, integer oder string\} angegeben wird.

Siehe [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Nicht-ganzzahliger numerischer Wert, Ganzzahlwert, Zeichenfolgenwert oder Boolescher Wert, der als Abfrageparameter verwendet wird. Wird nur verwendet, wenn parameterType = value ist.

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

