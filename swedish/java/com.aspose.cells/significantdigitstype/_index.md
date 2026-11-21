---
title: "SignificantDigitsType"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar typen av signifikanta siffror för utskrift av numeriska värden."
type: docs
url: /sv/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Representerar typen av signifikanta siffror för utskrift av numeriska värden.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15-siffror |
| [G_17](#G-17) | 17-siffror genom att formatera värdet med "G17". |
| [ROUNDING_17](#ROUNDING-17) | 17-siffror genom att avrunda värdet. |
## Metoder

| Metod | Beskrivning |
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


15-siffror

### G_17 {#G-17}
```
public static final int G_17
```


17-siffror genom att formatera värdet med "G17".

**Remarks**

För vissa double‑värden kan "G17" ge ett annat värde än det ursprungliga/litterala som användaren angav. Till exempel kommer double‑värdet 0.15 att skrivas ut som 0.14999999999999999; double‑värdet 1.0E-16 kommer att skrivas ut som 9.9999999999999998E-17. Ms Excel hanterar dessa värden inkonsekvent; den sparar 0.15 som 0.15 i xlsx‑filen, men för 1.0E-16 sparas värdet i xlsx‑filen som 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17-siffror genom att avrunda värdet.

**Remarks**

Denna typ skriver vanligtvis ut värdet som det ursprungliga/litterala som användaren angav. För 0.15 producerar den "0.15" och för 1.0E-16 producerar den "1.0E-16". Men det finns också vissa specialfall som kan ge andra värden än det litterala. Till exempel, när 208435494.96478021 avrundas till 17‑siffror ("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#"), blir resultatet 208435494.96478.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

