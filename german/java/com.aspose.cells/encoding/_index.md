---
title: "Encoding"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Zeichenkodierung dar."
type: docs
url: /de/java/com.aspose.cells/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

Stellt eine Zeichenkodierung dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.cells.Encoding-) | Bestimmt, ob das angegebene Encoding-Objekt gleich der aktuellen Instanz ist. |
| [equals(Object o)](#equals-java.lang.Object-) | Bestimmt, ob das angegebene Objekt gleich der aktuellen Instanz ist. |
| [getASCII()](#getASCII--) | Ruft eine Kodierung für den ASCII (7‑Bit)-Zeichensatz ab. |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Ruft eine Kodierung für das UTF‑16-Format mit Big‑Endian-Byte‑Reihenfolge ab. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Ruft eine Kodierung für die aktuelle ANSI‑Codepage des Betriebssystems ab. |
| [getEncoding(int codePage)](#getEncoding-int-) | Gibt die mit dem angegebenen Codepage‑Bezeichner verknüpfte Kodierung zurück. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Gibt eine Kodierung zurück, die mit dem angegebenen Zeichensatznamen verknüpft ist. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Gibt eine Kodierung zurück, die mit dem angegebenen Zeichensatzobjekt verknüpft ist. |
| [getUTF7()](#getUTF7--) | Liefert eine Kodierung für das UTF-7-Format. |
| [getUTF8()](#getUTF8--) | Liefert eine Kodierung für das UTF-8-Format. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | Liefert eine Kodierung für das UTF-8-Format ohne den UTF-8-Bezeichner. |
| [getUnicode()](#getUnicode--) | Liefert eine Kodierung für das UTF-16-Format unter Verwendung der Little-Endian-Byte-Reihenfolge. |
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


Bestimmt, ob das angegebene Encoding-Objekt gleich der aktuellen Instanz ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.cells/encoding) | Das Encoding-Objekt zum Vergleich mit der aktuellen Instanz. |

**Returns:**
boolean – true, wenn der Wert gleich der aktuellen Instanz ist; andernfalls false.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Bestimmt, ob das angegebene Objekt gleich der aktuellen Instanz ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt zum Vergleich mit der aktuellen Instanz. |

**Returns:**
boolean – true, wenn der Wert eine Instanz von Encoding ist und der aktuellen Instanz entspricht; andernfalls false.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


Ruft eine Kodierung für den ASCII (7‑Bit)-Zeichensatz ab.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


Ruft eine Kodierung für das UTF‑16-Format mit Big‑Endian-Byte‑Reihenfolge ab.

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


Ruft eine Kodierung für die aktuelle ANSI‑Codepage des Betriebssystems ab.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


Gibt die mit dem angegebenen Codepage‑Bezeichner verknüpfte Kodierung zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| codePage | int | Der Codepage-Bezeichner der bevorzugten Kodierung. -oder- 0, um die Standardkodierung zu verwenden. |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


Gibt eine Kodierung zurück, die mit dem angegebenen Zeichensatznamen verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| charsetName | java.lang.String | angegebener Zeichensatzname |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


Gibt eine Kodierung zurück, die mit dem angegebenen Zeichensatzobjekt verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| charset | java.nio.charset.Charset | angegebenes Zeichensatzobjekt |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


Liefert eine Kodierung für das UTF-7-Format.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


Liefert eine Kodierung für das UTF-8-Format.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


Liefert eine Kodierung für das UTF-8-Format ohne den UTF-8-Bezeichner.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


Liefert eine Kodierung für das UTF-16-Format unter Verwendung der Little-Endian-Byte-Reihenfolge.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

