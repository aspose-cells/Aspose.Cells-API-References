---
title: "Encoding"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una codificación de caracteres."
type: docs
url: /es/java/com.aspose.cells/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

Representa una codificación de caracteres.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.cells.Encoding-) | Determina si el objeto Encoding especificado es igual a la instancia actual. |
| [equals(Object o)](#equals-java.lang.Object-) | Determina si el Object especificado es igual a la instancia actual. |
| [getASCII()](#getASCII--) | Obtiene una codificación para el conjunto de caracteres ASCII (7 bits). |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Obtiene una codificación para el formato UTF-16 usando el orden de bytes big endian. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Obtiene una codificación para la página de códigos ANSI actual del sistema operativo. |
| [getEncoding(int codePage)](#getEncoding-int-) | Devuelve la codificación asociada al identificador de página de códigos especificado. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Devuelve una codificación asociada al nombre de conjunto de caracteres especificado. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Devuelve una codificación asociada al objeto charset especificado. |
| [getUTF7()](#getUTF7--) | Obtiene una codificación para el formato UTF-7. |
| [getUTF8()](#getUTF8--) | Obtiene una codificación para el formato UTF-8. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | Obtiene una codificación para el formato UTF-8 sin el identificador UTF-8. |
| [getUnicode()](#getUnicode--) | Obtiene una codificación para el formato UTF-16 usando el orden de bytes little endian. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Encoding() {#Encoding--}
```
public Encoding()
```


### equals(Encoding other) {#equals-com.aspose.cells.Encoding-}
```
public boolean equals(Encoding other)
```


Determina si el objeto Encoding especificado es igual a la instancia actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.cells/encoding) | El objeto Encoding para comparar con la instancia actual. |

**Returns:**
boolean - true si el valor es igual a la instancia actual; de lo contrario, false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Determina si el Object especificado es igual a la instancia actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El Object para comparar con la instancia actual. |

**Returns:**
boolean - true si el valor es una instancia de Encoding y es igual a la instancia actual; de lo contrario, false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


Obtiene una codificación para el conjunto de caracteres ASCII (7 bits).

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


Obtiene una codificación para el formato UTF-16 usando el orden de bytes big endian.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-16 format using the big endian byte
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefault() {#getDefault--}
```
public static Encoding getDefault()
```


Obtiene una codificación para la página de códigos ANSI actual del sistema operativo.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


Devuelve la codificación asociada al identificador de página de códigos especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| codePage | int | El identificador de página de códigos de la codificación preferida. -or- 0, para usar la codificación predeterminada. |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


Devuelve una codificación asociada al nombre de conjunto de caracteres especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| charsetName | java.lang.String | nombre de charset especificado |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


Devuelve una codificación asociada al objeto charset especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| charset | java.nio.charset.Charset | objeto charset especificado |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


Obtiene una codificación para el formato UTF-7.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


Obtiene una codificación para el formato UTF-8.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


Obtiene una codificación para el formato UTF-8 sin el identificador UTF-8.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


Obtiene una codificación para el formato UTF-16 usando el orden de bytes little endian.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-16 format using the little endian byte
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

