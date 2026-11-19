---
title: "GridPictureCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridpicturecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPictureCollection
```

封装一组 [GridPicture](../../com.aspose.gridweb/gridpicture) 对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | 向集合中添加一张图片。 |
| [add(int upperLeftRow, int upperLeftColumn, String fileName)](#add-int-int-java.lang.String-) | 向集合中添加一张图片。 |
| [add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | 向集合中添加一张图片。 |
| [clear()](#clear--) | 清除所有图片。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [GridPicture](../../com.aspose.gridweb/gridpicture) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取枚举器的大小 |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | 获取行枚举器 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int param_int)](#removeAt-int-) | 删除特定索引处的形状 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | int | 左上行索引。 |
| upperLeftColumn | int | 左上列索引。 |
| lowerRightRow | int | 右下行索引 |
| lowerRightColumn | int | 右下列索引 |
| fileName | java.lang.String | 图像文件名。 |

**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) 对象索引。
### add(int upperLeftRow, int upperLeftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | int | 左上行索引。 |
| upperLeftColumn | int | 左上列索引。 |
| fileName | java.lang.String | 图像文件名。 |

**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) 对象索引。
### add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | int | 左上行索引。 |
| upperLeftColumn | int | 左上列索引。 |
| fileName | java.lang.String | 图像文件名。 |
| widthScale | int | 图像宽度的比例，百分比。 |
| heightScale | int | 图像高度的比例，百分比。 |

**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) 对象索引。
### clear() {#clear--}
```
public void clear()
```


清除所有图片。

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
public GridPicture get(int index)
```


获取指定索引处的 [GridPicture](../../com.aspose.gridweb/gridpicture) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[GridPicture](../../com.aspose.gridweb/gridpicture) - The element at the specified index.
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


获取枚举器的大小

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取行枚举器

**Returns:**
java.util.Iterator - 行枚举器
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int param_int) {#removeAt-int-}
```
public void removeAt(int param_int)
```


删除特定索引处的形状

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| param_int | int |  |

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

