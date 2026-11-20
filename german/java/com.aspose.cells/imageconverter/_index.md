---
title: "ImageConverter"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Konverter zum Konvertieren von Vorlagendateien in Bilder."
type: docs
url: /de/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

Konverter zum Konvertieren von Vorlagendateien in Bilder.

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | Konvertiert die Vorlagendatei in Bilder |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Konvertiert die Vorlagendatei in Bilder |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Konvertiert die Vorlagendatei in Bilder. |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```


Konvertiert die Vorlagendatei in Bilder

**Remarks**

Beim Konvertieren in ein Bildformat, das mehrere Seiten unterstützt (wie z. B. TIFF), wird die angegebene [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) oder [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) direkt für das resultierende Bild verwendet.

Für andere Bildtypen, wenn die Speicheroptionen einen Stream als Ausgabe angegeben haben, werden alle resultierenden Bilder in denselben Stream gespeichert. Andernfalls werden die Ausgabedateien aus der angegebenen Ausgabedatei der Speicheroptionen erstellt, indem die Sequenznummer des Blatts und des Teilsegments angehängt wird. Zum Beispiel, wenn die angegebene Ausgabedatei Image.png ist, werden die erzeugten Bilddateien Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ... sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Optionen für Eingabe und Laden |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Optionen für Ausgabe und Speichern |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


Konvertiert die Vorlagendatei in Bilder

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Optionen für Eingabe und Laden |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Optionen zum Speichern. Seine Ausgabe ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) oder [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) hat keine Wirkung, da alle Ausgaben durch den Parameter "provider" festgelegt werden. |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | Provider der Speicheroptionen zum Speichern der erzeugten Bilder |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Konvertiert die Vorlagendatei in Bilder.

**Remarks**

Die Ausgabedateien werden aus der angegebenen Ergebnisdatei erstellt, indem die Sequenznummer des Blatts und des Teilsegments angehängt wird. Zum Beispiel, wenn die angegebene Ausgabedatei Image.png ist, werden die erzeugten Bilddateien Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ... sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | java.lang.String | Die Vorlagendatei, die in Bilder konvertiert werden soll. |
| resultFile | java.lang.String | Die resultierende Datei (Namensmuster) für erzeugte Bilder. |

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

