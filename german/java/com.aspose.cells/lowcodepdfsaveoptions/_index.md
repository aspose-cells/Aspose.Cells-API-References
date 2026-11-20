---
title: "LowCodePdfSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Optionen zum Speichern von PDF auf Low‑Code‑Weise."
type: docs
url: /de/java/com.aspose.cells/lowcodepdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodePdfSaveOptions extends LowCodeSaveOptions
```

Optionen zum Speichern von PDF auf Low‑Code‑Weise.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LowCodePdfSaveOptions()](#LowCodePdfSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Ermittelt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten. |
| [getOutputStream()](#getOutputStream--) | Ermittelt den Stream zum Schreiben der erzeugten Daten. |
| [getPdfOptions()](#getPdfOptions--) | Die Optionen zum Speichern der PDF-Datei. |
| [getSaveFormat()](#getSaveFormat--) | Das Speicherformat für die Ausgabe. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Legt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten fest. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Legt den Stream zum Schreiben der erzeugten Daten fest. |
| [setPdfOptions(PdfSaveOptions value)](#setPdfOptions-com.aspose.cells.PdfSaveOptions-) | Die Optionen zum Speichern der PDF-Datei. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Das Speicherformat für die Ausgabe. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodePdfSaveOptions() {#LowCodePdfSaveOptions--}
```
public LowCodePdfSaveOptions()
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
### getPdfOptions() {#getPdfOptions--}
```
public PdfSaveOptions getPdfOptions()
```


Die Optionen zum Speichern der PDF-Datei.

**Returns:**
[PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Das Speicherformat für die Ausgabe. Für die Konvertierung zu PDF kann nur [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF) verwendet werden.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

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

### setPdfOptions(PdfSaveOptions value) {#setPdfOptions-com.aspose.cells.PdfSaveOptions-}
```
public void setPdfOptions(PdfSaveOptions value)
```


Die Optionen zum Speichern der PDF-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions) |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Das Speicherformat für die Ausgabe. Für die Konvertierung zu PDF kann nur [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF) verwendet werden.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

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

