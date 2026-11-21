---
title: "LowCodeSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Alternativ för att spara genererade resultat på ett low‑code‑sätt."
type: docs
url: /sv/java/com.aspose.cells/lowcodesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class LowCodeSaveOptions
```

Alternativ för att spara genererade resultat på ett low‑code‑sätt.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [LowCodeSaveOptions()](#LowCodeSaveOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Hämtar filen (med sökväg om behövs) för att spara den genererade datan. |
| [getOutputStream()](#getOutputStream--) | Hämtar strömmen för att skriva den genererade datan till. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar sparformatet för utdata. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Ställer in filen (med sökväg om behövs) för att spara den genererade datan. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Ställer in strömmen för att skriva den genererade datan till. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Ställer in sparformatet för utdata. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptions() {#LowCodeSaveOptions--}
```
public LowCodeSaveOptions()
```


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
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Hämtar filen (med sökväg om behövs) för att spara den genererade datan. När denna egenskap sätts till ett värde som inte är null eller en tom sträng, kommer [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) att ignoreras.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Hämtar strömmen för att skriva den genererade datan till. När egenskapen sätts till ett värde annat än null, kommer [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) att ignoreras.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar sparformatet för utdata. Generellt, för specifika processer i lågkodsläge, är endast vissa specifika format tillåtna. Ange det korrekta formatet för motsvarande process, annars kan oväntade resultat eller till och med undantag uppstå.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
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




### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Anger filen (med sökväg om behövs) för att spara den genererade datan. När egenskapen sätts till ett värde annat än null eller en tom sträng, kommer [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) att ignoreras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Anger strömmen för att skriva den genererade datan till. När egenskapen sätts till ett värde annat än null, kommer [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) att ignoreras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Ställer in sparformatet för utdata. Generellt, för specifika processer i lågkodsläge, är endast vissa specifika format tillåtna. Ange det korrekta formatet för motsvarande process, annars kan oväntade resultat eller till och med undantag uppstå.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

