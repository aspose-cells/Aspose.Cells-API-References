---
title: "LowCodeHtmlSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Optionen zum Speichern von HTML auf Low‑Code‑Weise."
type: docs
url: /de/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

Optionen zum Speichern von HTML auf Low‑Code‑Weise.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | Die allgemeinen Optionen zum Speichern von HTML. |
| [getOutputFile()](#getOutputFile--) | Ermittelt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten. |
| [getOutputStream()](#getOutputStream--) | Ermittelt den Stream zum Schreiben der erzeugten Daten. |
| [getSaveFormat()](#getSaveFormat--) | Ruft das Format der Tabelle ab. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | Die allgemeinen Optionen zum Speichern von HTML. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Legt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten fest. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Legt den Stream zum Schreiben der erzeugten Daten fest. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Legt das Format der Tabelle fest. |
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


Die allgemeinen Optionen zum Speichern von HTML.

**Remarks**

Wenn eine [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)-Instanz angegeben wird, wird die [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\\#getSaveFormat--) überschrieben (falls sie zuvor angegeben wurde).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Ermittelt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) ignoriert.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Ermittelt den Stream zum Schreiben der erzeugten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) ignoriert.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ruft das Format der Tabelle ab.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Beim Ändern dieser Eigenschaft wird das durch [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\\#getHtmlOptions--) angegebene Speicherformat ignoriert (falls es zuvor angegeben wurde).

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


Die allgemeinen Optionen zum Speichern von HTML.

**Remarks**

Wenn eine [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)-Instanz angegeben wird, wird die [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\\#getSaveFormat--) überschrieben (falls sie zuvor angegeben wurde).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Legt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten fest. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) ignoriert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Legt den Stream zum Schreiben der erzeugten Daten fest. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) ignoriert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Legt das Format der Tabelle fest.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Beim Ändern dieser Eigenschaft wird das durch [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\\#getHtmlOptions--) angegebene Speicherformat ignoriert (falls es zuvor angegeben wurde).

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

