---
title: "FileFormatUtil"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Fournit des méthodes utilitaires pour convertir les énumérations de format de fichier en chaînes ou en extensions de fichier et inversement."
type: docs
url: /fr/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Fournit des méthodes utilitaires pour convertir les énumérations de format de fichier en chaînes ou en extensions de fichier et inversement.
## Méthodes

| Méthode | Description |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un flux. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un flux. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un fichier. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un fichier. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Convertit une extension de nom de fichier en une valeur SaveFormat. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Conversion du format de fichier en format d'enregistrement. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Renvoie vrai si l'extension est .xlt, .xltX, .xltm, .ots. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Convertit une valeur énumérée de format de chargement en une extension de fichier. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Convertit une valeur LoadFormat en une valeur SaveFormat si possible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Convertit une valeur énumérée de format d'enregistrement en une extension de fichier. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Convertit une valeur SaveFormat en une valeur LoadFormat si possible. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un flux. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | Le mot de passe pour les fichiers ooxml chiffrés. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un fichier.

**Remarks**

Ne prend en charge que la vérification de certains fichiers avec une signature magique. S'il n'y a pas de signature magique, nous ne pouvons pas détecter précisément le format du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un fichier.

**Remarks**

Ne prend en charge que la vérification de certains fichiers avec une signature magique. S'il n'y a pas de signature magique, nous ne pouvons pas détecter précisément le format du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| password | java.lang.String | Le mot de passe pour les fichiers ooxml chiffrés. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Convertit une extension de nom de fichier en une valeur SaveFormat.

**Remarks**

Si l'extension ne peut pas être reconnue, renvoie [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extension | java.lang.String | L'extension du fichier. Peut être avec ou sans point initial. Insensible à la casse. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Conversion du format de fichier en format d'enregistrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). Le type de format de fichier. |

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


Renvoie vrai si l'extension est .xlt, .xltX, .xltm, .ots.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Convertit une valeur énumérée de format de chargement en une extension de fichier.

**Remarks**

Si cela ne peut pas être converti, renvoie null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Le format de fichier chargé. |

**Returns:**
java.lang.String - L'extension renvoyée est une chaîne en minuscules avec un point initial.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Convertit une valeur LoadFormat en une valeur SaveFormat si possible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Le format de chargement. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). Le format d'enregistrement.
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


Convertit une valeur énumérée de format d'enregistrement en une extension de fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). Le format d'enregistrement. |

**Returns:**
java.lang.String - L'extension renvoyée est une chaîne en minuscules avec un point initial.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Convertit une valeur SaveFormat en une valeur LoadFormat si possible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le format d'enregistrement. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). Le format de chargement
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


Détecte et renvoie les informations sur le format d'un fichier Excel stocké dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | Le mot de passe pour les fichiers ooxml chiffrés. |

**Returns:**
boolean - Renvoie si le mot de passe est corrigé.
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

