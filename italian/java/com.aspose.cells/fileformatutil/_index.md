---
title: "FileFormatUtil"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Fornisce metodi di utilità per convertire gli enum di formato file in stringhe o estensioni di file e viceversa."
type: docs
url: /it/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Fornisce metodi di utilità per convertire gli enum di formato file in stringhe o estensioni di file e viceversa.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Rileva e restituisce le informazioni su un formato di Excel memorizzato in uno stream. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Rileva e restituisce le informazioni su un formato di Excel memorizzato in uno stream. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Rileva e restituisce le informazioni su un formato di Excel memorizzato in un file. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Rileva e restituisce le informazioni su un formato di Excel memorizzato in un file. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Converte un'estensione di nome file in un valore SaveFormat. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Conversione del formato file in formato di salvataggio. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Restituisce true se l'estensione è .xlt, .xltX, .xltm,.ots. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Converte un valore enumerato di LoadFormat in un'estensione di file. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Converte un valore LoadFormat in un valore SaveFormat, se possibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Converte un valore enumerato di SaveFormat in un'estensione di file. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Converte un valore SaveFormat in un valore LoadFormat, se possibile. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Rileva e restituisce le informazioni su un formato di Excel memorizzato in uno stream. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Rileva e restituisce le informazioni su un formato di Excel memorizzato in uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Lo stream |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Rileva e restituisce le informazioni su un formato di Excel memorizzato in uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | La password per i file ooxml crittografati. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Rileva e restituisce le informazioni su un formato di Excel memorizzato in un file.

**Remarks**

Supporta solo il controllo di alcuni file con firma magica. Se non c'è firma magica, non possiamo rilevare con precisione il formato del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Rileva e restituisce le informazioni su un formato di Excel memorizzato in un file.

**Remarks**

Supporta solo il controllo di alcuni file con firma magica. Se non c'è firma magica, non possiamo rilevare con precisione il formato del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| password | java.lang.String | La password per i file ooxml crittografati. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Converte un'estensione di nome file in un valore SaveFormat.

**Remarks**

Se l'estensione non può essere riconosciuta, restituisce [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extension | java.lang.String | L'estensione del file. Può essere con o senza il punto iniziale. Non sensibile al maiuscolo/minuscolo. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Conversione del formato file in formato di salvataggio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). Il tipo di formato file. |

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


Restituisce true se l'estensione è .xlt, .xltX, .xltm,.ots.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Converte un valore enumerato di LoadFormat in un'estensione di file.

**Remarks**

Se non può essere convertito, restituisce null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Il formato del file caricato. |

**Returns:**
java.lang.String - L'estensione restituita è una stringa in minuscolo con un punto iniziale.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Converte un valore LoadFormat in un valore SaveFormat, se possibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Il formato di caricamento. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). Il formato di salvataggio.
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


Converte un valore enumerato di SaveFormat in un'estensione di file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). Il formato di salvataggio. |

**Returns:**
java.lang.String - L'estensione restituita è una stringa in minuscolo con un punto iniziale.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Converte un valore SaveFormat in un valore LoadFormat, se possibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Il formato di salvataggio. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). Il formato di caricamento
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


Rileva e restituisce le informazioni su un formato di Excel memorizzato in uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | La password per i file ooxml crittografati. |

**Returns:**
boolean - Restituisce se la password è corretta.
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

