---
title: "Encodage"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un encodage de caractères."
type: docs
url: /fr/java/com.aspose.cells/encoding/
---

**Inheritance:**
java.lang.Object
```
public class Encoding
```

Représente un encodage de caractères.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Encoding()](#Encoding--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Encoding other)](#equals-com.aspose.cells.Encoding-) | Détermine si l'objet Encoding spécifié est égal à l'instance actuelle. |
| [equals(Object o)](#equals-java.lang.Object-) | Détermine si l'objet spécifié est égal à l'instance actuelle. |
| [getASCII()](#getASCII--) | Obtient un encodage pour le jeu de caractères ASCII (7 bits). |
| [getBigEndianUnicode()](#getBigEndianUnicode--) | Obtient un encodage pour le format UTF-16 en utilisant l'ordre des octets big endian. |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Obtient un encodage pour la page de codes ANSI actuelle du système d'exploitation. |
| [getEncoding(int codePage)](#getEncoding-int-) | Renvoie l'encodage associé à l'identifiant de page de codes spécifié. |
| [getEncoding(String charsetName)](#getEncoding-java.lang.String-) | Renvoie un encodage associé au nom de jeu de caractères spécifié. |
| [getEncoding(Charset charset)](#getEncoding-java.nio.charset.Charset-) | Renvoie un encodage associé à l'objet charset spécifié. |
| [getUTF7()](#getUTF7--) | Obtient un encodage pour le format UTF-7. |
| [getUTF8()](#getUTF8--) | Obtient un encodage pour le format UTF-8. |
| [getUTF8NoBOM()](#getUTF8NoBOM--) | Obtient un encodage pour le format UTF-8 sans l'identifiant UTF-8. |
| [getUnicode()](#getUnicode--) | Obtient un encodage pour le format UTF-16 en utilisant l'ordre des octets little endian. |
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


Détermine si l'objet Encoding spécifié est égal à l'instance actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [Encoding](../../com.aspose.cells/encoding) | L'objet Encoding à comparer avec l'instance actuelle. |

**Returns:**
booléen - vrai si la valeur est égale à l'instance actuelle ; sinon, faux.
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Détermine si l'objet spécifié est égal à l'instance actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à comparer avec l'instance actuelle. |

**Returns:**
booléen - vrai si la valeur est une instance de Encoding et est égale à l'instance actuelle ; sinon, faux.
### getASCII() {#getASCII--}
```
public static Encoding getASCII()
```


Obtient un encodage pour le jeu de caractères ASCII (7 bits).

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the ASCII (7-bit) character set.
### getBigEndianUnicode() {#getBigEndianUnicode--}
```
public static Encoding getBigEndianUnicode()
```


Obtient un encodage pour le format UTF-16 en utilisant l'ordre des octets big endian.

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


Obtient un encodage pour la page de codes ANSI actuelle du système d'exploitation.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - An encoding for the operating system's current ANSI code page.
### getEncoding(int codePage) {#getEncoding-int-}
```
public static Encoding getEncoding(int codePage)
```


Renvoie l'encodage associé à l'identifiant de page de codes spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| codePage | int | L'identifiant de la page de code de l'encodage préféré. -ou- 0, pour utiliser l'encodage par défaut. |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified code page.
### getEncoding(String charsetName) {#getEncoding-java.lang.String-}
```
public static Encoding getEncoding(String charsetName)
```


Renvoie un encodage associé au nom de jeu de caractères spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| charsetName | java.lang.String | nom du charset spécifié |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset name.
### getEncoding(Charset charset) {#getEncoding-java.nio.charset.Charset-}
```
public static Encoding getEncoding(Charset charset)
```


Renvoie un encodage associé à l'objet charset spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| charset | java.nio.charset.Charset | objet charset spécifié |

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - The Encoding object associated with the specified charset object.
### getUTF7() {#getUTF7--}
```
public static Encoding getUTF7()
```


Obtient un encodage pour le format UTF-7.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-7 format.
### getUTF8() {#getUTF8--}
```
public static Encoding getUTF8()
```


Obtient un encodage pour le format UTF-8.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format.
### getUTF8NoBOM() {#getUTF8NoBOM--}
```
public static Encoding getUTF8NoBOM()
```


Obtient un encodage pour le format UTF-8 sans l'identifiant UTF-8.

**Returns:**
[Encoding](../../com.aspose.cells/encoding) - A Encoding object for the UTF-8 format without UTF-8 identifier.
### getUnicode() {#getUnicode--}
```
public static Encoding getUnicode()
```


Obtient un encodage pour le format UTF-16 en utilisant l'ordre des octets little endian.

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

