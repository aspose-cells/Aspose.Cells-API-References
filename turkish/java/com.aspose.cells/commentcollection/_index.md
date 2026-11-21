---
title: "CommentCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/commentcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CommentCollection extends CollectionBase
```

[Comment](../../com.aspose.cells/comment) nesnelerinin bir koleksiyonunu kapsüller.

**Example**

```
         Workbook workbook = new Workbook();
 
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //do your business
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Koleksiyona bir yorum ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String cellName)](#add-java.lang.String-) | Koleksiyona bir yorum ekler. |
| [addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)](#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | İş parçacıklı bir yorum ekler. |
| [addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)](#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | İş parçacıklı bir yorum ekler. |
| [clear()](#clear--) | Tüm yorumları kaldırır; |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [Comment](../../com.aspose.cells/comment) öğesini alır. |
| [get(int row, int column)](#get-int-int-) | Belirtilen satır indeksi ve sütun indeksindeki [Comment](../../com.aspose.cells/comment) öğesini alır. |
| [get(String cellName)](#get-java.lang.String-) | Belirtilen hücredeki [Comment](../../com.aspose.cells/comment) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getThreadedComments(int row, int column)](#getThreadedComments-int-int-) | Satır ve sütun indeksine göre zincirli yorumları alır. |
| [getThreadedComments(String cellName)](#getThreadedComments-java.lang.String-) | Hücre adına göre zincirli yorumları alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [removeAt(int row, int column)](#removeAt-int-int-) | Belirli hücrenin yorumunu kaldırır. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Belirli hücrenin yorumunu kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Koleksiyona bir yorum ekler.

**Example**

```
         int commentIndex1 = comments.add(0, 0);
         Comment comment1 = comments.get(commentIndex1);
         comment1.setNote("First note.");
         comment1.getFont().setName("Times New Roman");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücre satır indeksi. |
| sütun | int | Hücre sütun indeksi. |

**Returns:**
int - [Comment](../../com.aspose.cells/comment) nesne indeksi.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


CollectionBase örneğine bir öğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğine eklenecek Nesne. |

**Returns:**
int - Yeni elemanın eklendiği konum.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Koleksiyona bir yorum ekler.

**Example**

```
         int commentIndex2 = comments.add("B2");
         Comment comment2 = comments.get(commentIndex2);
         comment2.setNote("Second note.");
         comment2.getFont().setName("Times New Roman");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |

**Returns:**
int - [Comment](../../com.aspose.cells/comment) nesne indeksi.
### addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author) {#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)
```


İş parçacıklı bir yorum ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücre satır indeksi. |
| sütun | int | Hücre sütun indeksi. |
| metin | java.lang.String | Yorumun metni |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | Bu zincirli yorumun kullanıcısı. |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) nesne indeksi.
### addThreadedComment(String cellName, String text, ThreadedCommentAuthor author) {#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)
```


İş parçacıklı bir yorum ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücrenin adı. |
| metin | java.lang.String | Yorumun metni |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | Bu zincirli yorumun kullanıcısı. |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) nesne indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm yorumları kaldırır;

**Example**

```
         comments.clear();
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Örneğin bu nesneyi içerip içermediğini döndürür

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | test nesnesi |

**Returns:**
boolean - Örneğin bu nesneyi içerip içermediği
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Comment get(int index)
```


Belirtilen indeksteki [Comment](../../com.aspose.cells/comment) öğesini alır.

**Example**

```
         Comment comment3 = comments.get(0);
         comment3.setNote("Three note.");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public Comment get(int row, int column)
```


Belirtilen satır indeksi ve sütun indeksindeki [Comment](../../com.aspose.cells/comment) öğesini alır.

**Example**

```
         Comment comment5 = comments.get(1,1);
         comment5.setNote("Five note.");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public Comment get(String cellName)
```


Belirtilen hücredeki [Comment](../../com.aspose.cells/comment) öğesini alır.

**Example**

```
         Comment comment4 = comments.get("B2");
         comment4.setNote("Four note.");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |

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


CollectionBase örneğinde bulunan eleman sayısını alır.

**Returns:**
int - CollectionBase örneğinde bulunan eleman sayısı.
### getThreadedComments(int row, int column) {#getThreadedComments-int-int-}
```
public ThreadedCommentCollection getThreadedComments(int row, int column)
```


Satır ve sütun indeksine göre zincirli yorumları alır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) - 
### getThreadedComments(String cellName) {#getThreadedComments-java.lang.String-}
```
public ThreadedCommentCollection getThreadedComments(String cellName)
```


Hücre adına göre zincirli yorumları alır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücrenin adı. |

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


CollectionBase örneğindeki belirli bir öğenin dizinini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |

**Returns:**
int - Değer listede bulunursa dizini; aksi takdirde -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür.

**Returns:**
java.util.Iterator - CollectionBase örneği için bir iterator.
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


Belirtilen dizindeki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak öğenin sıfır tabanlı dizini. |

### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


Belirli hücrenin yorumunu kaldırır.

**Example**

```
         comments.removeAt(1,1);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | sütun indeksi. |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


Belirli hücrenin yorumunu kaldırır.

**Example**

```
         comments.removeAt("B2");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Yorumu içeren hücrenin adı. |

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

