---
title: "CommentCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.cells/commentcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CommentCollection extends CollectionBase
```

Incapsula una raccolta di oggetti [Comment](../../com.aspose.cells/comment).

**Example**

```
         Workbook workbook = new Workbook();
 
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //do your business
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Aggiunge un commento alla raccolta. |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | Aggiunge un commento alla raccolta. |
| [addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)](#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Aggiunge un commento in thread. |
| [addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)](#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Aggiunge un commento in thread. |
| [clear()](#clear--) | Rimuove tutti i commenti; |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [Comment](../../com.aspose.cells/comment) all'indice specificato. |
| [get(int row, int column)](#get-int-int-) | Ottiene l'elemento [Comment](../../com.aspose.cells/comment) all'indice di riga e colonna specificati. |
| [get(String cellName)](#get-java.lang.String-) | Ottiene l'elemento [Comment](../../com.aspose.cells/comment) nella cella specificata. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [getThreadedComments(int row, int column)](#getThreadedComments-int-int-) | Ottiene i commenti in thread per indice di riga e colonna. |
| [getThreadedComments(String cellName)](#getThreadedComments-java.lang.String-) | Ottiene i commenti in thread per nome della cella. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento all'indice specificato. |
| [removeAt(int row, int column)](#removeAt-int-int-) | Rimuove il commento della cella specifica. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Rimuove il commento della cella specifica. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Aggiunge un commento alla raccolta.

**Example**

```
         int commentIndex1 = comments.add(0, 0);
         Comment comment1 = comments.get(commentIndex1);
         comment1.setNote("First note.");
         comment1.getFont().setName("Times New Roman");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga della cella. |
| colonna | int | Indice di colonna della cella. |

**Returns:**
int - indice dell'oggetto [Comment](../../com.aspose.cells/comment).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Aggiunge un commento alla raccolta.

**Example**

```
         int commentIndex2 = comments.add("B2");
         Comment comment2 = comments.get(commentIndex2);
         comment2.setNote("Second note.");
         comment2.getFont().setName("Times New Roman");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |

**Returns:**
int - indice dell'oggetto [Comment](../../com.aspose.cells/comment).
### addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author) {#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)
```


Aggiunge un commento in thread.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga della cella. |
| colonna | int | Indice di colonna della cella. |
| testo | java.lang.String | Il testo del commento |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | L'utente di questo commento in thread. |

**Returns:**
int - indice dell'oggetto [ThreadedComment](../../com.aspose.cells/threadedcomment).
### addThreadedComment(String cellName, String text, ThreadedCommentAuthor author) {#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)
```


Aggiunge un commento in thread.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Il nome della cella. |
| testo | java.lang.String | Il testo del commento |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | L'utente di questo commento in thread. |

**Returns:**
int - indice dell'oggetto [ThreadedComment](../../com.aspose.cells/threadedcomment).
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti i commenti;

**Example**

```
         comments.clear();
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Comment get(int index)
```


Ottiene l'elemento [Comment](../../com.aspose.cells/comment) all'indice specificato.

**Example**

```
         Comment comment3 = comments.get(0);
         comment3.setNote("Three note.");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public Comment get(int row, int column)
```


Ottiene l'elemento [Comment](../../com.aspose.cells/comment) all'indice di riga e colonna specificati.

**Example**

```
         Comment comment5 = comments.get(1,1);
         comment5.setNote("Five note.");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| colonna | int | Indice di colonna. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public Comment get(String cellName)
```


Ottiene l'elemento [Comment](../../com.aspose.cells/comment) nella cella specificata.

**Example**

```
         Comment comment4 = comments.get("B2");
         comment4.setNote("Four note.");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |

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


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### getThreadedComments(int row, int column) {#getThreadedComments-int-int-}
```
public ThreadedCommentCollection getThreadedComments(int row, int column)
```


Ottiene i commenti in thread per indice di riga e colonna.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) - 
### getThreadedComments(String cellName) {#getThreadedComments-java.lang.String-}
```
public ThreadedCommentCollection getThreadedComments(String cellName)
```


Ottiene i commenti in thread per nome della cella.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Il nome della cella. |

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


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
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


Rimuove l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento da rimuovere. |

### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


Rimuove il commento della cella specifica.

**Example**

```
         comments.removeAt(1,1);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | l'indice della colonna. |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


Rimuove il commento della cella specifica.

**Example**

```
         comments.removeAt("B2");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Il nome della cella che contiene un commento. |

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

