---
title: "SignificantDigitsType"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte dar."
type: docs
url: /de/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Stellt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte dar.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15 Stellen |
| [G_17](#G-17) | 17 Stellen durch Formatieren des Wertes mit "G17". |
| [ROUNDING_17](#ROUNDING-17) | 17 Stellen durch Runden des Wertes. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15 Stellen

### G_17 {#G-17}
```
public static final int G_17
```


17 Stellen durch Formatieren des Wertes mit "G17".

**Remarks**

Für einige Double‑Werte kann "G17" einen anderen Wert als den vom Benutzer eingegebenen Original‑/Literalwert liefern. Zum Beispiel wird der Double‑Wert 0.15 als 0.14999999999999999 ausgegeben; der Double‑Wert 1.0E-16 wird als 9.9999999999999998E-17 ausgegeben. Ms Excel behandelt diese Werte inkonsistent: Es speichert 0.15 als 0.15 in der xlsx‑Datei, aber für 1.0E-16 ist der gespeicherte Wert in der xlsx‑Datei 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17 Stellen durch Runden des Wertes.

**Remarks**

Dieser Typ gibt den Wert im Allgemeinen so aus, wie er vom Benutzer als Original‑/Literalwert eingegeben wurde. Für 0.15 erzeugt er "0.15" und für 1.0E-16 erzeugt er "1.0E-16". Es gibt jedoch einige Sonderfälle, die andere Werte als das Literal liefern können. Zum Beispiel wird beim Runden von 208435494.96478021 auf 17 Stellen ("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#") das Ergebnis 208435494.96478 sein.

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

