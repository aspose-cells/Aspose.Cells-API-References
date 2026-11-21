---
title: "Encoding"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir karakter kodlamasını temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

Bir karakter kodlamasını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.gridweb.Encoding-) | Belirtilen Encoding nesnesinin mevcut örnek ile eşit olup olmadığını belirler. |
| [equals(Object o)](#equals-java.lang.Object-) | Belirtilen Object nesnesinin mevcut örnek ile eşit olup olmadığını belirler. |
| [getASCII()](#getASCII--) | ASCII (7-bit) karakter kümesi için bir kodlama alır. |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Büyük endian bayt sırasını kullanarak UTF-16 formatı için bir kodlama alır. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | İşletim sisteminin mevcut ANSI kod sayfası için bir kodlama alır. |
| [getEncoding(int codePage)](#getEncoding-int-) | Belirtilen kod sayfası tanımlayıcısı ile ilişkili kodlamayı döndürür. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Belirtilen karakter kümesi adı ile ilişkili bir kodlamayı döndürür. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Belirtilen karakter kümesi nesnesiyle ilişkili bir kodlamayı döndürür. |
| [getUTF7()](#getUTF7--) | UTF-7 formatı için bir kodlama alır. |
| [getUTF8()](#getUTF8--) | UTF-8 formatı için bir kodlama alır. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | UTF-8 tanımlayıcısı olmadan UTF-8 formatı için bir kodlama alır. |
| [getUnicode()](#getUnicode--) | Küçük endian bayt sırasını kullanarak UTF-16 formatı için bir kodlama alır. |
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


Belirtilen Encoding nesnesinin mevcut örnek ile eşit olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.gridweb/encoding) | Mevcut örnek ile karşılaştırılacak Encoding nesnesi. |

**Returns:**
boolean - değer mevcut örnek ile eşitse true; aksi takdirde false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Belirtilen Object nesnesinin mevcut örnek ile eşit olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | Mevcut örnek ile karşılaştırılacak Nesne. |

**Returns:**
boolean - değer Encoding örneği ise ve mevcut örnek ile eşitse true; aksi takdirde false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


ASCII (7-bit) karakter kümesi için bir kodlama alır.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


Büyük endian bayt sırasını kullanarak UTF-16 formatı için bir kodlama alır.

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


İşletim sisteminin mevcut ANSI kod sayfası için bir kodlama alır.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


Belirtilen kod sayfası tanımlayıcısı ile ilişkili kodlamayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| codePage | int | Tercih edilen kodlamanın kod sayfası tanımlayıcısı. -veya- varsayılan kodlamayı kullanmak için 0. |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


Belirtilen karakter kümesi adı ile ilişkili bir kodlamayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| charsetName | java.lang.String | belirtilen karakter kümesi adı |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


Belirtilen karakter kümesi nesnesiyle ilişkili bir kodlamayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| charset | java.nio.charset.Charset | belirtilen karakter kümesi nesnesi |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


UTF-7 formatı için bir kodlama alır.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


UTF-8 formatı için bir kodlama alır.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


UTF-8 tanımlayıcısı olmadan UTF-8 formatı için bir kodlama alır.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


Küçük endian bayt sırasını kullanarak UTF-16 formatı için bir kodlama alır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

