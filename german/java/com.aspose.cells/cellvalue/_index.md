---
title: "CellValue"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Zellenwert und den entsprechenden Typ dar."
type: docs
url: /de/java/com.aspose.cells/cellvalue/
---

**Inheritance:**
java.lang.Object
```
public class CellValue
```

Stellt den Zellenwert und den entsprechenden Typ dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CellValue()](#CellValue--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Ermittelt den Typ des Zellwerts. |
| [getValue()](#getValue--) | Ermittelt den Zellwert. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setType(int value)](#setType-int-) | Setzt den Typ des Zellwerts. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Setzt den Zellwert. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellValue() {#CellValue--}
```
public CellValue()
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
### getType() {#getType--}
```
public int getType()
```


Ermittelt den Typ des Zellwerts.

Siehe [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Ermittelt den Zellwert.

**Remarks**

Der Wert muss vom korrekten Objekttyp sein, der der [getType()](../../com.aspose.cells/cellvalue\#getType--) entspricht:

| Typ | Value |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, jedes andere Objekt wird ignoriert |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | Fehlerzeichenfolge wie "\#VALUE!", "\#NAME?", ... |

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




### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Setzt den Typ des Zellwerts.

Siehe [CellValueType](../../com.aspose.cells/cellvaluetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Setzt den Zellwert.

**Remarks**

Der Wert muss vom korrekten Objekttyp sein, der der [getType()](../../com.aspose.cells/cellvalue\#getType--) entspricht:

| Typ | Value |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, jedes andere Objekt wird ignoriert |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | Fehlerzeichenfolge wie "\#VALUE!", "\#NAME?", ... |

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

