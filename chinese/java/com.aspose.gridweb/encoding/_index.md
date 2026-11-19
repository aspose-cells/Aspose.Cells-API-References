---
title: "编码"
second_title: "Aspose.Cells for Java API 参考"
description: "表示字符编码。"
type: docs
url: /zh/java/com.aspose.gridweb/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

表示字符编码。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.gridweb.Encoding-) | 确定指定的 Encoding 对象是否等于当前实例。 |
| [equals(Object o)](#equals-java.lang.Object-) | 确定指定的 Object 是否等于当前实例。 |
| [getASCII()](#getASCII--) | 获取 ASCII（7 位）字符集的编码。 |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | 获取使用大端字节序的 UTF-16 格式的编码。 |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | 获取操作系统当前 ANSI 代码页的编码。 |
| [getEncoding(int codePage)](#getEncoding-int-) | 返回与指定代码页标识符关联的编码。 |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | 返回与指定字符集名称关联的编码。 |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | 返回与指定字符集对象关联的编码。 |
| [getUTF7()](#getUTF7--) | 获取 UTF-7 格式的编码。 |
| [getUTF8()](#getUTF8--) | 获取 UTF-8 格式的编码。 |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | 获取不带 UTF-8 标识符的 UTF-8 格式编码。 |
| [getUnicode()](#getUnicode--) | 获取使用小端字节序的 UTF-16 格式编码。 |
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


确定指定的 Encoding 对象是否等于当前实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.gridweb/encoding) | 用于与当前实例比较的 Encoding 对象。 |

**Returns:**
boolean - 如果值等于当前实例则为 true；否则为 false。
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


确定指定的 Object 是否等于当前实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 用于与当前实例比较的 Object。 |

**Returns:**
boolean - 如果值是 Encoding 的实例且等于当前实例则为 true；否则为 false。
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


获取 ASCII（7 位）字符集的编码。

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


获取使用大端字节序的 UTF-16 格式的编码。

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


获取操作系统当前 ANSI 代码页的编码。

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


返回与指定代码页标识符关联的编码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| codePage | int | 首选编码的代码页标识符。-or- 0，使用默认编码。 |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


返回与指定字符集名称关联的编码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| charsetName | java.lang.String | 指定的字符集名称 |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


返回与指定字符集对象关联的编码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| charset | java.nio.charset.Charset | 指定的字符集对象 |

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


获取 UTF-7 格式的编码。

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


获取 UTF-8 格式的编码。

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


获取不带 UTF-8 标识符的 UTF-8 格式编码。

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


获取使用小端字节序的 UTF-16 格式编码。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

