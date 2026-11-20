---
title: "LowCodeImageSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Optionen zum Speichern von Bildern auf Low‑Code‑Weise."
type: docs
url: /de/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

Optionen zum Speichern von Bildern auf Low‑Code‑Weise.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | Die Optionen zum Rendern von Bildern. |
| [getOutputFile()](#getOutputFile--) | Ermittelt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten. |
| [getOutputStream()](#getOutputStream--) | Ermittelt den Stream zum Schreiben der erzeugten Daten. |
| [getSaveFormat()](#getSaveFormat--) | Liefert das Speicherformat. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Anbieter von Speicheroptionen zum Speichern generierter Bilder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | Die Optionen zum Rendern von Bildern. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Legt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten fest. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Legt den Stream zum Schreiben der erzeugten Daten fest. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Setzt das Speicherformat. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Anbieter von Speicheroptionen zum Speichern generierter Bilder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Die Optionen zum Rendern von Bildern.

**Remarks**

Wenn eine [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)-Instanz angegeben ist, wird die [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) überschrieben (falls sie zuvor angegeben wurde).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
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


Liefert das Speicherformat.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Wenn [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) angegeben wurde, ändert das Festlegen dieser Eigenschaft ebenfalls den Wert von [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--).

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


Anbieter von Speicheroptionen zum Speichern generierter Bilder.

**Remarks**

Die Ausgabe([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) oder [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) die von dieser Instanz angegeben wird, hat keine Wirkung, wenn diese Eigenschaft angegeben ist. Stattdessen wird die Ausgabe jedes erzeugten Bildes vom Anbieter festgelegt.

**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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




### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```


Die Optionen zum Rendern von Bildern.

**Remarks**

Wenn eine [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)-Instanz angegeben ist, wird die [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) überschrieben (falls sie zuvor angegeben wurde).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

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


Setzt das Speicherformat.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Wenn [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) angegeben wurde, ändert das Festlegen dieser Eigenschaft ebenfalls den Wert von [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


Anbieter von Speicheroptionen zum Speichern generierter Bilder.

**Remarks**

Die Ausgabe([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) oder [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) die von dieser Instanz angegeben wird, hat keine Wirkung, wenn diese Eigenschaft angegeben ist. Stattdessen wird die Ausgabe jedes erzeugten Bildes vom Anbieter festgelegt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |

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

