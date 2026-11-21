---
title: "LowCodeHtmlSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Alternativ för att spara HTML på ett low‑code‑sätt."
type: docs
url: /sv/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

Alternativ för att spara HTML på ett low‑code‑sätt.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | De allmänna alternativen för att spara HTML. |
| [getOutputFile()](#getOutputFile--) | Hämtar filen (med sökväg om behövs) för att spara den genererade datan. |
| [getOutputStream()](#getOutputStream--) | Hämtar strömmen för att skriva den genererade datan till. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar formatet för kalkylbladet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | De allmänna alternativen för att spara HTML. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Ställer in filen (med sökväg om behövs) för att spara den genererade datan. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Ställer in strömmen för att skriva den genererade datan till. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Ställer in formatet för kalkylbladet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


De allmänna alternativen för att spara HTML.

**Remarks**

När en [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) instans anges, kommer [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) att skrivas över (om den tidigare har angetts).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
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


Hämtar formatet för kalkylbladet.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

När denna egenskap ändras, kommer det sparformat som anges av [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) att ignoreras (om det tidigare har angetts).

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




### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```


De allmänna alternativen för att spara HTML.

**Remarks**

När en [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) instans anges, kommer [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) att skrivas över (om den tidigare har angetts).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

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


Ställer in formatet för kalkylbladet.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

När denna egenskap ändras, kommer det sparformat som anges av [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) att ignoreras (om det tidigare har angetts).

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

