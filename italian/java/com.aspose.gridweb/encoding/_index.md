---
title: "Encoding"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una codifica dei caratteri."
type: docs
url: /it/java/com.aspose.gridweb/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

Rappresenta una codifica dei caratteri.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.gridweb.Encoding-) | Determina se l'oggetto Encoding specificato è uguale all'istanza corrente. |
| [equals(Object o)](#equals-java.lang.Object-) | Determina se l'oggetto specificato è uguale all'istanza corrente. |
| [getASCII()](#getASCII--) | Ottiene una codifica per il set di caratteri ASCII (7 bit). |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Ottiene una codifica per il formato UTF-16 utilizzando l'ordine dei byte big endian. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Ottiene una codifica per la pagina di codice ANSI corrente del sistema operativo. |
| [getEncoding(int codePage)](#getEncoding-int-) | Restituisce la codifica associata all'identificatore di pagina di codice specificato. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Restituisce una codifica associata al nome del set di caratteri specificato. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Restituisce una codifica associata all'oggetto charset specificato. |
| [getUTF7()](#getUTF7--) | Ottiene una codifica per il formato UTF-7. |
| [getUTF8()](#getUTF8--) | Ottiene una codifica per il formato UTF-8. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | Ottiene una codifica per il formato UTF-8 senza l'identificatore UTF-8. |
| [getUnicode()](#getUnicode--) | Ottiene una codifica per il formato UTF-16 utilizzando l'ordine dei byte little endian. |
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


### equals(Encoding other) {#equals-com.aspose.gridweb.Encoding-}
```
public boolean equals(Encoding other)
```


Determina se l'oggetto Encoding specificato è uguale all'istanza corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.gridweb/encoding) | L'oggetto Encoding da confrontare con l'istanza corrente. |

**Returns:**
boolean - true se il valore è uguale all'istanza corrente; altrimenti, false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Determina se l'oggetto specificato è uguale all'istanza corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'oggetto da confrontare con l'istanza corrente. |

**Returns:**
boolean - true se il valore è un'istanza di Encoding ed è uguale all'istanza corrente; altrimenti, false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


Ottiene una codifica per il set di caratteri ASCII (7 bit).

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


Ottiene una codifica per il formato UTF-16 utilizzando l'ordine dei byte big endian.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-16 format using the big endian byte
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


Ottiene una codifica per la pagina di codice ANSI corrente del sistema operativo.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


Restituisce la codifica associata all'identificatore di pagina di codice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| codePage | int | L'identificatore della pagina di codice della codifica preferita. -or- 0, per utilizzare la codifica predefinita. |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


Restituisce una codifica associata al nome del set di caratteri specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| charsetName | java.lang.String | nome charset specificato |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


Restituisce una codifica associata all'oggetto charset specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| charset | java.nio.charset.Charset | oggetto charset specificato |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


Ottiene una codifica per il formato UTF-7.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


Ottiene una codifica per il formato UTF-8.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


Ottiene una codifica per il formato UTF-8 senza l'identificatore UTF-8.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


Ottiene una codifica per il formato UTF-16 utilizzando l'ordine dei byte little endian.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-16 format using the little endian byte
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

