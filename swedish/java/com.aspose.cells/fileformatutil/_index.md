---
title: "FileFormatUtil"
second_title: "Aspose.Cells för Java API-referens"
description: "Tillhandahåller hjälpfunktioner för att konvertera filformat‑enum till strängar eller filändelser och tillbaka."
type: docs
url: /sv/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Tillhandahåller hjälpfunktioner för att konvertera filformat‑enum till strängar eller filändelser och tillbaka.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Detekterar och returnerar information om ett format för en Excel som lagras i en ström. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Detekterar och returnerar information om ett format för en Excel som lagras i en ström. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Detekterar och returnerar information om ett format för en Excel som lagras i en fil. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Detekterar och returnerar information om ett format för en Excel som lagras i en fil. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Konverterar en filnamnsändelse till ett SaveFormat-värde. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Konverterar filformat till sparaformat. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Returnerar true om ändelsen är .xlt, .xltX, .xltm,.ots. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Konverterar ett uppräknat load-formatvärde till en filändelse. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Konverterar ett LoadFormat-värde till ett SaveFormat-värde om möjligt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Konverterar ett uppräknat sparaformatvärde till en filändelse. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Konverterar ett SaveFormat-värde till ett LoadFormat-värde om möjligt. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Detekterar och returnerar information om ett format för en Excel som lagras i en ström. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Detekterar och returnerar information om ett format för en Excel som lagras i en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Strömmen |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Detekterar och returnerar information om ett format för en Excel som lagras i en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| lösenord | java.lang.String | Lösenordet för krypterade ooxml-filer. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Detekterar och returnerar information om ett format för en Excel som lagras i en fil.

**Remarks**

Stöder endast kontroll av vissa filer med magisk signatur. Om det inte finns någon magisk signatur kan vi inte exakt upptäcka filformatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Detekterar och returnerar information om ett format för en Excel som lagras i en fil.

**Remarks**

Stöder endast kontroll av vissa filer med magisk signatur. Om det inte finns någon magisk signatur kan vi inte exakt upptäcka filformatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| lösenord | java.lang.String | Lösenordet för krypterade ooxml-filer. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
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
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Konverterar en filnamnsändelse till ett SaveFormat-värde.

**Remarks**

Om filändelsen inte kan identifieras, returneras [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filändelse | java.lang.String | Filändelsen. Kan vara med eller utan en inledande punkt. Skiftlägesokänslig. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Konverterar filformat till sparaformat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). Filformatstypen. |

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


Returnerar true om ändelsen är .xlt, .xltX, .xltm,.ots.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filändelse | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Konverterar ett uppräknat load-formatvärde till en filändelse.

**Remarks**

Om den inte kan konverteras, returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Det inlästa filformatet. |

**Returns:**
java.lang.String - Den returnerade filändelsen är en gemenersträng med en inledande punkt.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Konverterar ett LoadFormat-värde till ett SaveFormat-värde om möjligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Inläsningsformatet. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). Sparaformatet.
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


Konverterar ett uppräknat sparaformatvärde till en filändelse.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). Sparaformatet. |

**Returns:**
java.lang.String - Den returnerade filändelsen är en gemenersträng med en inledande punkt.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Konverterar ett SaveFormat-värde till ett LoadFormat-värde om möjligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Sparaformatet. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). Inläsningsformatet
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


Detekterar och returnerar information om ett format för en Excel som lagras i en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| lösenord | java.lang.String | Lösenordet för krypterade ooxml-filer. |

**Returns:**
boolean - Returnerar om lösenordet är korrigerat.
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

