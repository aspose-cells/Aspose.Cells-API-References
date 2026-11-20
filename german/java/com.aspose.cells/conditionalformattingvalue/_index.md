---
title: "ConditionalFormattingValue"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Beschreibt die Werte der Interpolationspunkte in einer gradient scale dataBar oder iconSet."
type: docs
url: /de/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Beschreibt die Werte der Interpolationspunkte in einer Verlaufs-Skala, Datenleiste oder Symbolsatz.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Gibt den Typ dieses ConditionalFormattingValue-Objekts zurück. |
| [getValue()](#getValue--) | Gibt den Wert dieses ConditionalFormattingValue-Objekts zurück. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Ruft das Größer‑als‑oder‑gleich‑Flag ab. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Setzt das Größer‑als‑oder‑gleich‑Flag. |
| [setType(int value)](#setType-int-) | Setzt den Typ dieses bedingten Formatierungswertobjekts. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Setzt den Wert dieses bedingten Formatierungswertobjekts. |
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
### getType() {#getType--}
```
public int getType()
```


Ruft den Typ dieses bedingten Formatierungswertobjekts ab. Das Setzen des Typs auf FormatConditionValueType.Min oder FormatConditionValueType.Max setzt "Value" automatisch auf null.

Siehe [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Ruft den Wert dieses bedingten Formatierungswertobjekts ab. Es sollte zusammen mit Type verwendet werden.

**Remarks**

Wenn der Wert ein String ist und mit "=" beginnt, wird er als Formel verarbeitet, andernfalls wird er als einfacher Wert verarbeitet.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


Ruft das Größer‑als‑oder‑gleich‑Flag ab. Nur für Symbolsets verwenden, bestimmt, ob dieser Schwellenwert den Größer‑als‑oder‑gleich‑Operator verwendet. 'false' bedeutet, dass 'größer als' anstelle von 'größer als oder gleich' verwendet wird. Der Standardwert ist true.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


Setzt das Größer‑als‑oder‑gleich‑Flag. Nur für Symbolsets verwenden, bestimmt, ob dieser Schwellenwert den Größer‑als‑oder‑gleich‑Operator verwendet. 'false' bedeutet, dass 'größer als' anstelle von 'größer als oder gleich' verwendet wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Setzt den Typ dieses bedingten Formatierungswertobjekts. Das Setzen des Typs auf FormatConditionValueType.Min oder FormatConditionValueType.Max setzt "Value" automatisch auf null.

Siehe [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Setzt den Wert dieses bedingten Formatierungswertobjekts. Es sollte zusammen mit Type verwendet werden.

**Remarks**

Wenn der Wert ein String ist und mit "=" beginnt, wird er als Formel verarbeitet, andernfalls wird er als einfacher Wert verarbeitet.

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

