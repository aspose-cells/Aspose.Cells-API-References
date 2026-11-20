---
title: "CommentCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/commentcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CommentCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [Comment](../../com.aspose.cells/comment).

**Example**

```
         Workbook workbook = new Workbook();
 
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //do your business
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Добавляет комментарий в коллекцию. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | Добавляет комментарий в коллекцию. |
| [addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)](#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Добавляет ветвящийся комментарий. |
| [addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)](#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | Добавляет ветвящийся комментарий. |
| [clear()](#clear--) | Удаляет все комментарии; |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [Comment](../../com.aspose.cells/comment) по указанному индексу. |
| [get(int row, int column)](#get-int-int-) | Получает элемент [Comment](../../com.aspose.cells/comment) по указанному индексу строки и индексу столбца. |
| [get(String cellName)](#get-java.lang.String-) | Получает элемент [Comment](../../com.aspose.cells/comment) по указанной ячейке. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [getThreadedComments(int row, int column)](#getThreadedComments-int-int-) | Получает ветвящиеся комментарии по индексу строки и столбца. |
| [getThreadedComments(String cellName)](#getThreadedComments-java.lang.String-) | Получает ветвящиеся комментарии по имени ячейки. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент по указанному индексу. |
| [removeAt(int row, int column)](#removeAt-int-int-) | Удаляет комментарий конкретной ячейки. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Удаляет комментарий конкретной ячейки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Добавляет комментарий в коллекцию.

**Example**

```
         int commentIndex1 = comments.add(0, 0);
         Comment comment1 = comments.get(commentIndex1);
         comment1.setNote("First note.");
         comment1.getFont().setName("Times New Roman");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки ячейки. |
| столбец | int | Индекс столбца ячейки. |

**Returns:**
int - [Comment](../../com.aspose.cells/comment) индекс объекта.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Добавляет комментарий в коллекцию.

**Example**

```
         int commentIndex2 = comments.add("B2");
         Comment comment2 = comments.get(commentIndex2);
         comment2.setNote("Second note.");
         comment2.getFont().setName("Times New Roman");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |

**Returns:**
int - [Comment](../../com.aspose.cells/comment) индекс объекта.
### addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author) {#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)
```


Добавляет ветвящийся комментарий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки ячейки. |
| столбец | int | Индекс столбца ячейки. |
| текст | java.lang.String | Текст комментария |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | Пользователь этого ветвящегося комментария. |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) индекс объекта.
### addThreadedComment(String cellName, String text, ThreadedCommentAuthor author) {#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)
```


Добавляет ветвящийся комментарий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |
| текст | java.lang.String | Текст комментария |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | Пользователь этого ветвящегося комментария. |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) индекс объекта.
### clear() {#clear--}
```
public void clear()
```


Удаляет все комментарии;

**Example**

```
         comments.clear();
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Comment get(int index)
```


Получает элемент [Comment](../../com.aspose.cells/comment) по указанному индексу.

**Example**

```
         Comment comment3 = comments.get(0);
         comment3.setNote("Three note.");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public Comment get(int row, int column)
```


Получает элемент [Comment](../../com.aspose.cells/comment) по указанному индексу строки и индексу столбца.

**Example**

```
         Comment comment5 = comments.get(1,1);
         comment5.setNote("Five note.");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public Comment get(String cellName)
```


Получает элемент [Comment](../../com.aspose.cells/comment) по указанной ячейке.

**Example**

```
         Comment comment4 = comments.get("B2");
         comment4.setNote("Four note.");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |

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


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### getThreadedComments(int row, int column) {#getThreadedComments-int-int-}
```
public ThreadedCommentCollection getThreadedComments(int row, int column)
```


Получает ветвящиеся комментарии по индексу строки и столбца.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) - 
### getThreadedComments(String cellName) {#getThreadedComments-java.lang.String-}
```
public ThreadedCommentCollection getThreadedComments(String cellName)
```


Получает ветвящиеся комментарии по имени ячейки.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |

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


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
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


Удаляет элемент по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента, который нужно удалить. |

### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


Удаляет комментарий конкретной ячейки.

**Example**

```
         comments.removeAt(1,1);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | индекс столбца. |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


Удаляет комментарий конкретной ячейки.

**Example**

```
         comments.removeAt("B2");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки, содержащей комментарий. |

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

