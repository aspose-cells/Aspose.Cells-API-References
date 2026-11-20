---
title: "Encoding"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет кодировку символов."
type: docs
url: /ru/java/com.aspose.gridweb/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

Представляет кодировку символов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.gridweb.Encoding-) | Определяет, равен ли указанный объект Encoding текущему экземпляру. |
| [equals(Object o)](#equals-java.lang.Object-) | Определяет, равен ли указанный объект Object текущему экземпляру. |
| [getASCII()](#getASCII--) | Получает кодировку для набора символов ASCII (7‑бит). |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Получает кодировку для формата UTF-16 с использованием порядка байтов big endian. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Получает кодировку для текущей ANSI‑страницы кодов операционной системы. |
| [getEncoding(int codePage)](#getEncoding-int-) | Возвращает кодировку, связанную с указанным идентификатором страницы кодов. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Возвращает кодировку, связанную с указанным именем набора символов. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Возвращает кодировку, связанную с указанным объектом набора символов. |
| [getUTF7()](#getUTF7--) | Получает кодировку для формата UTF-7. |
| [getUTF8()](#getUTF8--) | Получает кодировку для формата UTF-8. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | Получает кодировку для формата UTF-8 без идентификатора UTF-8. |
| [getUnicode()](#getUnicode--) | Получает кодировку для формата UTF-16, используя порядок байтов little endian. |
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


Определяет, равен ли указанный объект Encoding текущему экземпляру.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.gridweb/encoding) | Объект Encoding для сравнения с текущим экземпляром. |

**Returns:**
boolean - true, если значение равно текущему экземпляру; иначе false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Определяет, равен ли указанный объект Object текущему экземпляру.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект для сравнения с текущим экземпляром. |

**Returns:**
boolean - true, если значение является экземпляром Encoding и равно текущему экземпляру; иначе false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


Получает кодировку для набора символов ASCII (7‑бит).

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


Получает кодировку для формата UTF-16 с использованием порядка байтов big endian.

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


Получает кодировку для текущей ANSI‑страницы кодов операционной системы.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


Возвращает кодировку, связанную с указанным идентификатором страницы кодов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| codePage | int | Идентификатор кодовой страницы предпочтительной кодировки. -or- 0, чтобы использовать кодировку по умолчанию. |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


Возвращает кодировку, связанную с указанным именем набора символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| charsetName | java.lang.String | указанное имя набора символов |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


Возвращает кодировку, связанную с указанным объектом набора символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| charset | java.nio.charset.Charset | указанный объект набора символов |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


Получает кодировку для формата UTF-7.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


Получает кодировку для формата UTF-8.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


Получает кодировку для формата UTF-8 без идентификатора UTF-8.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


Получает кодировку для формата UTF-16, используя порядок байтов little endian.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

