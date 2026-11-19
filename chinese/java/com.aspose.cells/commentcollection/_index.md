---
title: "CommentCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/commentcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CommentCollection extends CollectionBase
```

封装一个 [Comment](../../com.aspose.cells/comment) 对象的集合。

**Example**

```
         Workbook workbook = new Workbook();
 
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //do your business
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | 向集合添加评论。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String cellName)](#add-java.lang.String-) | 向集合添加评论。 |
| [addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)](#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | 添加一个线程评论。 |
| [addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)](#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-) | 添加一个线程评论。 |
| [clear()](#clear--) | 移除所有评论； |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [Comment](../../com.aspose.cells/comment) 元素。 |
| [get(int row, int column)](#get-int-int-) | 获取指定行索引和列索引处的 [Comment](../../com.aspose.cells/comment) 元素。 |
| [get(String cellName)](#get-java.lang.String-) | 获取指定单元格处的 [Comment](../../com.aspose.cells/comment) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getThreadedComments(int row, int column)](#getThreadedComments-int-int-) | 按行列索引获取线程评论。 |
| [getThreadedComments(String cellName)](#getThreadedComments-java.lang.String-) | 按单元格名称获取线程评论。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [removeAt(int row, int column)](#removeAt-int-int-) | 移除特定单元格的评论。 |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | 移除特定单元格的评论。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


向集合添加评论。

**Example**

```
         int commentIndex1 = comments.add(0, 0);
         Comment comment1 = comments.get(commentIndex1);
         comment1.setNote("First note.");
         comment1.getFont().setName("Times New Roman");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格行索引。 |
| 列 | int | 单元格列索引。 |

**Returns:**
int - [Comment](../../com.aspose.cells/comment) 对象索引。
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


向 CollectionBase 实例添加一个项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要添加到 CollectionBase 实例的对象。 |

**Returns:**
int - 新元素插入的位置。
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


向集合添加评论。

**Example**

```
         int commentIndex2 = comments.add("B2");
         Comment comment2 = comments.get(commentIndex2);
         comment2.setNote("Second note.");
         comment2.getFont().setName("Times New Roman");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |

**Returns:**
int - [Comment](../../com.aspose.cells/comment) 对象索引。
### addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author) {#addThreadedComment-int-int-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(int row, int column, String text, ThreadedCommentAuthor author)
```


添加一个线程评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格行索引。 |
| 列 | int | 单元格列索引。 |
| 文本 | java.lang.String | 注释的文本 |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | 此线程注释的用户。 |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) 对象索引。
### addThreadedComment(String cellName, String text, ThreadedCommentAuthor author) {#addThreadedComment-java.lang.String-java.lang.String-com.aspose.cells.ThreadedCommentAuthor-}
```
public int addThreadedComment(String cellName, String text, ThreadedCommentAuthor author)
```


添加一个线程评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格的名称。 |
| 文本 | java.lang.String | 注释的文本 |
| author | [ThreadedCommentAuthor](../../com.aspose.cells/threadedcommentauthor) | 此线程注释的用户。 |

**Returns:**
int - [ThreadedComment](../../com.aspose.cells/threadedcomment) 对象索引。
### clear() {#clear--}
```
public void clear()
```


移除所有评论；

**Example**

```
         comments.clear();
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


返回实例是否包含此对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 测试对象 |

**Returns:**
boolean - 实例是否包含此对象
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Comment get(int index)
```


获取指定索引处的 [Comment](../../com.aspose.cells/comment) 元素。

**Example**

```
         Comment comment3 = comments.get(0);
         comment3.setNote("Three note.");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public Comment get(int row, int column)
```


获取指定行索引和列索引处的 [Comment](../../com.aspose.cells/comment) 元素。

**Example**

```
         Comment comment5 = comments.get(1,1);
         comment5.setNote("Five note.");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[Comment](../../com.aspose.cells/comment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public Comment get(String cellName)
```


获取指定单元格处的 [Comment](../../com.aspose.cells/comment) 元素。

**Example**

```
         Comment comment4 = comments.get("B2");
         comment4.setNote("Four note.");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |

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


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### getThreadedComments(int row, int column) {#getThreadedComments-int-int-}
```
public ThreadedCommentCollection getThreadedComments(int row, int column)
```


按行列索引获取线程评论。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection) - 
### getThreadedComments(String cellName) {#getThreadedComments-java.lang.String-}
```
public ThreadedCommentCollection getThreadedComments(String cellName)
```


按单元格名称获取线程评论。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格的名称。 |

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


确定 CollectionBase 实例中特定项的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 确定 CollectionBase 实例中特定项的索引。 |

**Returns:**
int - 如果在列表中找到该值则返回其索引；否则返回 -1。
### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
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


移除指定索引处的项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除的项的零基索引。 |

### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


移除特定单元格的评论。

**Example**

```
         comments.removeAt(1,1);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


移除特定单元格的评论。

**Example**

```
         comments.removeAt("B2");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 包含注释的单元格名称。 |

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

