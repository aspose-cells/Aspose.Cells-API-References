---
title: "ThreadedCommentAuthorCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla personer."
type: docs
url: /sv/java/com.aspose.cells/threadedcommentauthorcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ThreadedCommentAuthorCollection extends CollectionBase
```

Representerar alla personer.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [ThreadedCommentAuthorCollection()](#ThreadedCommentAuthorCollection--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String name, String userId, String providerId)](#add-java.lang.String-java.lang.String-java.lang.String-) | Lägger till en person för trådkommentar. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar personen som skapar trådade kommentarer. |
| [get(String name)](#get-java.lang.String-) | Hämtar personen som skapar trådade kommentarer. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getCurrentPerson()](#getCurrentPerson--) | Hämtar den aktuella användaren. |
| [hashCode()](#hashCode--) |  |
| [indexOf(ThreadedCommentAuthor author)](#indexOf-com.aspose.cells.ThreadedCommentAuthor-) | Hämtar indexet för ThreadedCommentAuthor-objektet |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort objektet på det angivna indexet. |
| [setCurrentPerson(ThreadedCommentAuthor value)](#setCurrentPerson-com.aspose.cells.ThreadedCommentAuthor-) | Ställer in den aktuella användaren. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadedCommentAuthorCollection() {#ThreadedCommentAuthorCollection--}
```
public ThreadedCommentAuthorCollection()
```


### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### add(String name, String userId, String providerId) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String name, String userId, String providerId)
```


Lägger till en person för trådkommentar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på personen. |
| userId | java.lang.String |  |
| providerId | java.lang.String | Leverantörens id |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från CollectionBase-instansen.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public ThreadedCommentAuthor get(int index)
```


Hämtar personen som skapar trådade kommentarer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet |

**Returns:**
[ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) - 
### get(String name) {#get-java.lang.String-}
```
public ThreadedCommentAuthor get(String name)
```


Hämtar personen som skapar trådade kommentarer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Författarens namn. |

**Returns:**
[ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### getCurrentPerson() {#getCurrentPerson--}
```
public ThreadedCommentAuthor getCurrentPerson()
```


Hämtar den aktuella användaren.

**Returns:**
[ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(ThreadedCommentAuthor author) {#indexOf-com.aspose.cells.ThreadedCommentAuthor-}
```
public int indexOf(ThreadedCommentAuthor author)
```


Hämtar indexet för ThreadedCommentAuthor-objektet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | ThreadedCommentAuthor-objektet |

**Returns:**
int – Indexet i ThreadedCommentAuthor-samlingen
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort objektet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för objektet som ska tas bort. |

### setCurrentPerson(ThreadedCommentAuthor value) {#setCurrentPerson-com.aspose.cells.ThreadedCommentAuthor-}
```
public void setCurrentPerson(ThreadedCommentAuthor value)
```


Ställer in den aktuella användaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) |  |

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

