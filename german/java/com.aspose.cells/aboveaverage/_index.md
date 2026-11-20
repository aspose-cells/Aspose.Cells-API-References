---
title: "AboveAverage"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Beschreiben Sie die AboveAverage‑Bedingte‑Formatierungsregel."
type: docs
url: /de/java/com.aspose.cells/aboveaverage/
---

**Inheritance:**
java.lang.Object
```
public class AboveAverage
```

Beschreiben Sie die AboveAverage‑Bedingte‑Formatierungsregel. Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AboveAverage()](#AboveAverage--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getStdDev()](#getStdDev--) | Liefert die Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel einbezogen werden. |
| [hashCode()](#hashCode--) |  |
| [isAboveAverage()](#isAboveAverage--) | Liefert das Flag, das angibt, ob die Regel eine "über dem Durchschnitt"‑Regel ist. |
| [isEqualAverage()](#isEqualAverage--) | Liefert das Flag, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnitt selbst einschließen oder von diesem Wert ausschließen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAboveAverage(boolean value)](#setAboveAverage-boolean-) | Setzt das Flag, das angibt, ob die Regel eine "über dem Durchschnitt"‑Regel ist. |
| [setEqualAverage(boolean value)](#setEqualAverage-boolean-) | Setzt das Flag, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnitt selbst einschließen oder von diesem Wert ausschließen. |
| [setStdDev(int value)](#setStdDev-int-) | Setzt die Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel einbezogen werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AboveAverage() {#AboveAverage--}
```
public AboveAverage()
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
### getStdDev() {#getStdDev--}
```
public int getStdDev()
```


Liefert die Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel einbezogen werden. Der Eingabewert muss zwischen 0 und 3 liegen (einschließlich 0 und 3). Wird dieser Wert auf 0 gesetzt, bedeutet dies, dass stdDev nicht festgelegt ist. Der Standardwert ist 0.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAboveAverage() {#isAboveAverage--}
```
public boolean isAboveAverage()
```


Liefert das Flag, das angibt, ob die Regel eine "über dem Durchschnitt"‑Regel ist. 'true' bedeutet 'über dem Durchschnitt'. Der Standardwert ist true.

**Returns:**
boolean
### isEqualAverage() {#isEqualAverage--}
```
public boolean isEqualAverage()
```


Liefert das Flag, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnitt selbst einschließen oder von diesem Wert ausschließen. 'true' bedeutet, den Durchschnittswert in die Kriterien einzuschließen. Der Standardwert ist false.

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




### setAboveAverage(boolean value) {#setAboveAverage-boolean-}
```
public void setAboveAverage(boolean value)
```


Setzt das Flag, das angibt, ob die Regel eine "über dem Durchschnitt"‑Regel ist. 'true' bedeutet 'über dem Durchschnitt'. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEqualAverage(boolean value) {#setEqualAverage-boolean-}
```
public void setEqualAverage(boolean value)
```


Setzt das Flag, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnitt selbst einschließen oder von diesem Wert ausschließen. 'true' bedeutet, den Durchschnittswert in die Kriterien einzuschließen. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStdDev(int value) {#setStdDev-int-}
```
public void setStdDev(int value)
```


Setzt die Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel einbezogen werden. Der Eingabewert muss zwischen 0 und 3 liegen (einschließlich 0 und 3). Wird dieser Wert auf 0 gesetzt, bedeutet dies, dass stdDev nicht festgelegt ist. Der Standardwert ist 0.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

