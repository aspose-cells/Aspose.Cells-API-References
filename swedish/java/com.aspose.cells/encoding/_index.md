---
title: "Encoding"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en teckenkodning."
type: docs
url: /sv/java/com.aspose.cells/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

Representerar en teckenkodning.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.cells.Encoding-) | Bestämmer om det angivna Encoding-objektet är lika med den aktuella instansen. |
| [equals(Object o)](#equals-java.lang.Object-) | Bestämmer om det angivna objektet är lika med den aktuella instansen. |
| [getASCII()](#getASCII--) | Hämtar en kodning för ASCII (7-bitars) teckenuppsättningen. |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Hämtar en kodning för UTF-16-formatet med big endian-byteordning. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Hämtar en kodning för operativsystemets aktuella ANSI-kodningssida. |
| [getEncoding(int codePage)](#getEncoding-int-) | Returnerar kodningen som är associerad med den angivna kodsidens identifierare. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Returnerar en kodning som är associerad med det angivna teckenuppsättningsnamnet. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Returnerar en kodning som är associerad med det angivna teckenuppsättningsobjektet. |
| [getUTF7()](#getUTF7--) | Hämtar en kodning för UTF-7-formatet. |
| [getUTF8()](#getUTF8--) | Hämtar en kodning för UTF-8-formatet. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | Hämtar en kodning för UTF-8-formatet utan UTF-8-identifieraren. |
| [getUnicode()](#getUnicode--) | Hämtar en kodning för UTF-16-formatet med little endian-byteordning. |
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


Bestämmer om det angivna Encoding-objektet är lika med den aktuella instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.cells/encoding) | Encoding-objektet att jämföra med den aktuella instansen. |

**Returns:**
boolean - true om värdet är lika med den aktuella instansen; annars false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Bestämmer om det angivna objektet är lika med den aktuella instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet att jämföra med den aktuella instansen. |

**Returns:**
boolean - true om värdet är en instans av Encoding och är lika med den aktuella instansen; annars false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


Hämtar en kodning för ASCII (7-bitars) teckenuppsättningen.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


Hämtar en kodning för UTF-16-formatet med big endian-byteordning.

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


Hämtar en kodning för operativsystemets aktuella ANSI-kodningssida.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


Returnerar kodningen som är associerad med den angivna kodsidens identifierare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| codePage | int | Kodsididentifieraren för den föredragna kodningen. -eller- 0, för att använda standardkodningen. |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


Returnerar en kodning som är associerad med det angivna teckenuppsättningsnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| charsetName | java.lang.String | angivet teckenuppsättningsnamn |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


Returnerar en kodning som är associerad med det angivna teckenuppsättningsobjektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| charset | java.nio.charset.Charset | angivet teckenuppsättningsobjekt |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


Hämtar en kodning för UTF-7-formatet.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


Hämtar en kodning för UTF-8-formatet.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


Hämtar en kodning för UTF-8-formatet utan UTF-8-identifieraren.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


Hämtar en kodning för UTF-16-formatet med little endian-byteordning.

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

