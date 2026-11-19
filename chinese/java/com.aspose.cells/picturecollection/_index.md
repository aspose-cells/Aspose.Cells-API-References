---
title: "PictureCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

封装一个 [Picture](../../com.aspose.cells/picture) 对象的集合。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get PictureCollection
         PictureCollection pictures = workbook.getWorksheets().get(0).getPictures();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | 向集合中添加一张图片。 |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | 向集合中添加一张图片。 |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | 向集合中添加一张图片。 |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | 向集合中添加一张图片。 |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | 向集合中添加一张图片。 |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | 向集合中添加一张图片。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | 对该范围拍照。 |
| [clear()](#clear--) | 清除所有图片。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [Picture](../../com.aspose.cells/picture) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 删除特定索引处的形状 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| bottomRow | int | 右下行索引 |
| rightColumn | int | 右下列索引 |
| stream | java.io.InputStream | 包含图像数据的流对象。 |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) 对象索引。
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


向集合中添加一张图片。

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| bottomRow | int | 右下行索引 |
| rightColumn | int | 右下列索引 |
| fileName | java.lang.String | 图像文件名。 |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) 对象索引。
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| stream | java.io.InputStream | 包含图像数据的流对象。 |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) 对象索引。
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| stream | java.io.InputStream | 包含图像数据的流对象。 |
| widthScale | int | 图像宽度的比例，百分比。 |
| heightScale | int | 图像高度的比例，百分比。 |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) 对象索引。
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


向集合中添加一张图片。

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| fileName | java.lang.String | 图像文件名。 |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) 对象索引。
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


向集合中添加一张图片。

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| fileName | java.lang.String | 图像文件名。 |
| widthScale | int | 图像宽度的比例，百分比。 |
| heightScale | int | 图像高度的比例，百分比。 |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) 对象索引。
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
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


对该范围拍照。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 此图片的行索引。 |
| 列 | int | 此图片的列索引。 |
| 范围 | java.lang.String | 需要拍照的区域 |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


清除所有图片。

**Example**

```
         //clear
         pictures.clear();
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
public Picture get(int index)
```


获取指定索引处的 [Picture](../../com.aspose.cells/picture) 元素。

**Example**

```
         //get picture collection
         //PictureCollection pictures = workbook.Worksheets[0].Pictures;
         //add a picture
         int index = pictures.add(1, 1, "image.png");
         //get the picture
         Picture pic = pictures.get(index);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - The element at the specified index.
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


删除特定索引处的形状

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

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

