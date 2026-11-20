---
title: "FileFormatUtil"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Bietet Hilfsmethoden zum Konvertieren von Dateiformat-Enums in Zeichenketten oder Dateierweiterungen und zurück."
type: docs
url: /de/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Bietet Hilfsmethoden zum Konvertieren von Dateiformat-Enums in Zeichenketten oder Dateierweiterungen und zurück.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einem Stream gespeichert ist. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einem Stream gespeichert ist. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einer Datei gespeichert ist. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einer Datei gespeichert ist. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Konvertiert eine Dateinamenerweiterung in einen SaveFormat-Wert. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Konvertiert das Dateiformat in das Speicherformat. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Gibt true zurück, wenn die Erweiterung .xlt, .xltX, .xltm oder .ots ist. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Konvertiert einen aufgelisteten Load-Format-Wert in eine Dateierweiterung. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Konvertiert einen LoadFormat-Wert in einen SaveFormat-Wert, falls möglich. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Konvertiert einen aufgelisteten Save-Format-Wert in eine Dateierweiterung. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Konvertiert einen SaveFormat-Wert in einen LoadFormat-Wert, falls möglich. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einem Stream gespeichert ist. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einem Stream gespeichert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Stream |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einem Stream gespeichert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| Passwort | java.lang.String | Das Passwort für verschlüsselte ooxml-Dateien. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einer Datei gespeichert ist.

**Remarks**

Unterstützt nur die Prüfung einiger Dateien mit magischer Signatur. Wenn keine magische Signatur vorhanden ist, können wir das Dateiformat nicht genau erkennen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einer Datei gespeichert ist.

**Remarks**

Unterstützt nur die Prüfung einiger Dateien mit magischer Signatur. Wenn keine magische Signatur vorhanden ist, können wir das Dateiformat nicht genau erkennen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| Passwort | java.lang.String | Das Passwort für verschlüsselte ooxml-Dateien. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
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
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Konvertiert eine Dateinamenerweiterung in einen SaveFormat-Wert.

**Remarks**

Wenn die Erweiterung nicht erkannt werden kann, wird [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN) zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extension | java.lang.String | Die Dateierweiterung. Kann mit oder ohne führenden Punkt angegeben werden. Groß-/Kleinschreibung wird ignoriert. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Konvertiert das Dateiformat in das Speicherformat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). Der Dateiformattyp. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
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
### isTemplateFormat(String extension) {#isTemplateFormat-java.lang.String-}
```
public static boolean isTemplateFormat(String extension)
```


Gibt true zurück, wenn die Erweiterung .xlt, .xltX, .xltm oder .ots ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Konvertiert einen aufgelisteten Load-Format-Wert in eine Dateierweiterung.

**Remarks**

Wenn es nicht konvertiert werden kann, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Das geladene Dateiformat. |

**Returns:**
java.lang.String - Die zurückgegebene Erweiterung ist ein kleingeschriebener String mit einem führenden Punkt.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Konvertiert einen LoadFormat-Wert in einen SaveFormat-Wert, falls möglich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Das Ladeformat. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). Das Speicherformat.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveFormatToExtension(int format) {#saveFormatToExtension-int-}
```
public static String saveFormatToExtension(int format)
```


Konvertiert einen aufgelisteten Save-Format-Wert in eine Dateierweiterung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). Das Speicherformat. |

**Returns:**
java.lang.String - Die zurückgegebene Erweiterung ist ein kleingeschriebener String mit einem führenden Punkt.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Konvertiert einen SaveFormat-Wert in einen LoadFormat-Wert, falls möglich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Das Speicherformat. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). Das Ladeformat
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(InputStream stream, String password) {#verifyPassword-java.io.InputStream-java.lang.String-}
```
public static boolean verifyPassword(InputStream stream, String password)
```


Erkennt und gibt die Informationen über das Format einer Excel-Datei zurück, die in einem Stream gespeichert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| Passwort | java.lang.String | Das Passwort für verschlüsselte ooxml-Dateien. |

**Returns:**
boolean - Gibt zurück, ob das Passwort korrigiert ist.
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

