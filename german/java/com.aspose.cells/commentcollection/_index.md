---
title: "CommentCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.cells/commentcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CommentCollection extends CollectionBase
```

Kapselt eine Sammlung von [Comment](../../com.aspose.cells/comment)-Objekten.

**Example**

```
         Workbook workbook = new Workbook();
 
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //do your business
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Fügt der Sammlung einen Kommentar hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String cellName)](#add-java.lang.String-) | Fügt der Sammlung einen Kommentar hinzu. |
| [addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)](#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Fügt einen Thread‑Kommentar hinzu. |
| [addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)](#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Fügt einen Thread‑Kommentar hinzu. |
| [clear()](#clear--) | Entfernt alle Kommentare; |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liest das [Comment](../../com.aspose.cells/comment)-Element am angegebenen Index. |
| [get(int row, int column)](#get-int-int-) | Liest das [Comment](../../com.aspose.cells/comment)-Element am angegebenen Zeilenindex und Spaltenindex. |
| [get(String cellName)](#get-java.lang.String-) | Liefert das [Comment](../../com.aspose.cells/comment)-Element an der angegebenen Zelle. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getThreadedComments(int row, int column)](#getThreadedComments-int-int-) | Ruft die Threaded Comments nach Zeilen- und Spaltenindex ab. |
| [getThreadedComments(String cellName)](#getThreadedComments-java.lang.String-) | Ruft die Threaded Comments nach Zellnamen ab. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element am angegebenen Index. |
| [removeAt(int row, int column)](#removeAt-int-int-) | Entfernt den Kommentar der angegebenen Zelle. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Entfernt den Kommentar der angegebenen Zelle. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Fügt der Sammlung einen Kommentar hinzu.

**Example**

```
         int commentIndex1 = comments.add(0, 0);
         Comment comment1 = comments.get(commentIndex1);
         comment1.setNote("First note.");
         comment1.getFont().setName("Times New Roman");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der Zelle. |
| Spalte | int | Spaltenindex der Zelle. |

**Returns:**
int - [Comment](../../com.aspose.cells/comment)-Objektindex.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Fügt der Sammlung einen Kommentar hinzu.

**Example**

```
         int commentIndex2 = comments.add("B2");
         Comment comment2 = comments.get(commentIndex2);
         comment2.setNote("Second note.");
         comment2.getFont().setName("Times New Roman");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

**Returns:**
int - [Comment](../../com.aspose.cells/comment)-Objektindex.
### addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author) {#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)
```


Fügt einen Thread‑Kommentar hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der Zelle. |
| Spalte | int | Spaltenindex der Zelle. |
| Text | java.lang.String | Der Text des Kommentars |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | Der Benutzer dieses Threaded Comments. |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment)-Objektindex.
### addThreadedComment(String cellName, String text, ThreadedCommentAuthor author) {#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)
```


Fügt einen Thread‑Kommentar hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Der Name der Zelle. |
| Text | java.lang.String | Der Text des Kommentars |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | Der Benutzer dieses Threaded Comments. |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment)-Objektindex.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Kommentare;

**Example**

```
         comments.clear();
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Comment get(int index)
```


Liest das [Comment](../../com.aspose.cells/comment)-Element am angegebenen Index.

**Example**

```
         Comment comment3 = comments.get(0);
         comment3.setNote("Three note.");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public Comment get(int row, int column)
```


Liest das [Comment](../../com.aspose.cells/comment)-Element am angegebenen Zeilenindex und Spaltenindex.

**Example**

```
         Comment comment5 = comments.get(1,1);
         comment5.setNote("Five note.");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public Comment get(String cellName)
```


Liefert das [Comment](../../com.aspose.cells/comment)-Element an der angegebenen Zelle.

**Example**

```
         Comment comment4 = comments.get("B2");
         comment4.setNote("Four note.");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
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


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### getThreadedComments(int row, int column) {#getThreadedComments-int-int-}
```
public ThreadedCommentCollection getThreadedComments(int row, int column)
```


Ruft die Threaded Comments nach Zeilen- und Spaltenindex ab.

**Example**

```
         ThreadedCommentCollection threadedComments1 = comments.getThreadedComments(1, 1);
         for (int i = 0; i <threadedComments1.getCount(); ++i)
         {
             ThreadedComment tc = threadedComments1.get(i);
             String note = tc.getNotes();
         }
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) - 
### getThreadedComments(String cellName) {#getThreadedComments-java.lang.String-}
```
public ThreadedCommentCollection getThreadedComments(String cellName)
```


Ruft die Threaded Comments nach Zellnamen ab.

**Example**

```
         ThreadedCommentCollection threadedComments2 = comments.getThreadedComments("B2");
         for (int i = 0; i <threadedComments2.getCount(); ++i)
         {
             ThreadedComment tc = threadedComments2.get(i);
             String note = tc.getNotes();
         }
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Der Name der Zelle. |

**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) - 
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
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


Entfernt das Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des zu entfernenden Elements. |

### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


Entfernt den Kommentar der angegebenen Zelle.

**Example**

```
         comments.removeAt(1,1);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | der Spaltenindex. |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


Entfernt den Kommentar der angegebenen Zelle.

**Example**

```
         comments.removeAt("B2");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Der Name der Zelle, die einen Kommentar enthält. |

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

