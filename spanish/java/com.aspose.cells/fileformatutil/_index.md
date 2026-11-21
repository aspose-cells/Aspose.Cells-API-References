---
title: "FileFormatUtil"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Proporciona métodos utilitarios para convertir enumeraciones de formato de archivo a cadenas o extensiones de archivo y viceversa."
type: docs
url: /es/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Proporciona métodos utilitarios para convertir enumeraciones de formato de archivo a cadenas o extensiones de archivo y viceversa.
## Métodos

| Método | Descripción |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Detecta y devuelve la información sobre el formato de un Excel almacenado en un flujo. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Detecta y devuelve la información sobre el formato de un Excel almacenado en un flujo. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Detecta y devuelve la información sobre el formato de un Excel almacenado en un archivo. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Detecta y devuelve la información sobre el formato de un Excel almacenado en un archivo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Convierte una extensión de nombre de archivo en un valor SaveFormat. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Convirtiendo el formato de archivo a formato de guardado. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Devuelve verdadero si la extensión es .xlt, .xltX, .xltm, .ots. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Convierte un valor enumerado de formato de carga en una extensión de archivo. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Convierte un valor LoadFormat a un valor SaveFormat si es posible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Convierte un valor enumerado de formato de guardado en una extensión de archivo. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Convierte un valor SaveFormat a un valor LoadFormat si es posible. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Detecta y devuelve la información sobre el formato de un Excel almacenado en un flujo. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Detecta y devuelve la información sobre el formato de un Excel almacenado en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Detecta y devuelve la información sobre el formato de un Excel almacenado en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | La contraseña para archivos ooxml cifrados. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Detecta y devuelve la información sobre el formato de un Excel almacenado en un archivo.

**Remarks**

Solo admite la verificación de algunos archivos con firma mágica. Si no hay firma mágica, no podemos detectar con precisión el formato del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Detecta y devuelve la información sobre el formato de un Excel almacenado en un archivo.

**Remarks**

Solo admite la verificación de algunos archivos con firma mágica. Si no hay firma mágica, no podemos detectar con precisión el formato del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| password | java.lang.String | La contraseña para archivos ooxml cifrados. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Convierte una extensión de nombre de archivo en un valor SaveFormat.

**Remarks**

Si la extensión no puede ser reconocida, devuelve [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extension | java.lang.String | La extensión del archivo. Puede estar con o sin un punto inicial. No distingue entre mayúsculas y minúsculas. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Convirtiendo el formato de archivo a formato de guardado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). El tipo de formato de archivo. |

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


Devuelve verdadero si la extensión es .xlt, .xltX, .xltm, .ots.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Convierte un valor enumerado de formato de carga en una extensión de archivo.

**Remarks**

Si no se puede convertir, devuelve null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). El formato de archivo cargado. |

**Returns:**
java.lang.String - La extensión devuelta es una cadena en minúsculas con un punto inicial.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Convierte un valor LoadFormat a un valor SaveFormat si es posible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). El formato de carga. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). El formato de guardado.
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


Convierte un valor enumerado de formato de guardado en una extensión de archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). El formato de guardado. |

**Returns:**
java.lang.String - La extensión devuelta es una cadena en minúsculas con un punto inicial.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Convierte un valor SaveFormat a un valor LoadFormat si es posible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). El formato de guardado. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). El formato de carga
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


Detecta y devuelve la información sobre el formato de un Excel almacenado en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | La contraseña para archivos ooxml cifrados. |

**Returns:**
boolean - Devuelve si la contraseña es correcta.
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

