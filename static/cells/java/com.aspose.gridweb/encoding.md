##Encoding
Represents a character encoding.
**Inheritance:**
java.lang.Object
```
public class Encoding
```
Represents a character encoding.
## Constructors
| Constructor | Description |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.gridweb.Encoding-) | Determines whether the specified Encoding object is equal to the current instance. |
| [equals(Object o)](#equals-java.lang.Object-) | Determines whether the specified Object is equal to the current instance. |
| [getASCII()](#getASCII--) | Gets an encoding for the ASCII (7-bit) character set. |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Gets an encoding for the UTF-16 format using the big endian byte order. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Gets an encoding for the operating system's current ANSI code page. |
| [getEncoding(int codePage)](#getEncoding-int-) | Returns the encoding associated with the specified code page identifier. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Returns an encoding associated with the specified charset name. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Returns an encoding associated with the specified charset object. |
| [getUTF7()](#getUTF7--) | Gets an encoding for the UTF-7 format. |
| [getUTF8()](#getUTF8--) | Gets an encoding for the UTF-8 format. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | Gets an encoding for the UTF-8 format without the UTF-8 identifier. |
| [getUnicode()](#getUnicode--) | Gets an encoding for the UTF-16 format using the little endian byte order. |
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
Determines whether the specified Encoding object is equal to the current instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.gridweb/encoding) | The Encoding object to compare with the current instance. |
**Returns:**
boolean - true if value is equal to the current instance; otherwise, false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```
Determines whether the specified Object is equal to the current instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to compare with the current instance. |
**Returns:**
boolean - true if value is an instance of Encoding and is equal to the current instance; otherwise, false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```
Gets an encoding for the ASCII (7-bit) character set.
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```
Gets an encoding for the UTF-16 format using the big endian byte order.
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
Gets an encoding for the operating system's current ANSI code page.
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```
Returns the encoding associated with the specified code page identifier.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| codePage | int | The code page identifier of the preferred encoding. -or- 0, to use the default encoding. |
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```
Returns an encoding associated with the specified charset name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| charsetName | java.lang.String | specified charset name |
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```
Returns an encoding associated with the specified charset object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| charset | java.nio.charset.Charset | specified charset object |
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```
Gets an encoding for the UTF-7 format.
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```
Gets an encoding for the UTF-8 format.
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```
Gets an encoding for the UTF-8 format without the UTF-8 identifier.
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```
Gets an encoding for the UTF-16 format using the little endian byte order.
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
