---
title: "VbaModuleCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示以下列表"
type: docs
url: /zh/java/com.aspose.cells/vbamodulecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaModuleCollection extends CollectionBase
```

表示以下列表 [VbaModule](../../com.aspose.cells/vbamodule)

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Worksheet sheet)](#add-com.aspose.cells.Worksheet-) | 为工作表添加模块。 |
| [add(int type, String name)](#add-int-java.lang.String-) | 添加模块。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [addDesignerStorage(String name, byte[] data)](#addDesignerStorage-java.lang.String-byte---) |  |
| [addUserForm(String name, String codes, byte[] designerStorage)](#addUserForm-java.lang.String-java.lang.String-byte---) | 将用户窗体插入 VBA 项目。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取列表中的 [VbaModule](../../com.aspose.cells/vbamodule)。 |
| [get(String name)](#get-java.lang.String-) | 通过名称获取列表中的 [VbaModule](../../com.aspose.cells/vbamodule)。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getDesignerStorage(String name)](#getDesignerStorage-java.lang.String-) | 表示设计器的数据。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Worksheet sheet)](#remove-com.aspose.cells.Worksheet-) | 删除工作表的模块。 |
| [remove(String name)](#remove-java.lang.String-) | 通过名称删除模块 |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Worksheet sheet) {#add-com.aspose.cells.Worksheet-}
```
public int add(Worksheet sheet)
```


为工作表添加模块。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | 工作表 |

**Returns:**
int -
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


添加模块。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [VbaModuleType](../../com.aspose.cells/vbamoduletype)。模块的类型。 |
| 名称 | java.lang.String | 模块的名称。 |

**Returns:**
int -
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
### addDesignerStorage(String name, byte[] data) {#addDesignerStorage-java.lang.String-byte---}
```
public void addDesignerStorage(String name, byte[] data)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |
| 数据 | byte[] |  |

### addUserForm(String name, String codes, byte[] designerStorage) {#addUserForm-java.lang.String-java.lang.String-byte---}
```
public int addUserForm(String name, String codes, byte[] designerStorage)
```


将用户窗体插入 VBA 项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 用户窗体的名称 |
| 代码 | java.lang.String | 用户窗体的代码 |
| designerStorage | byte[] | 关于用户窗体的设计器设置 |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


从 CollectionBase 实例中移除所有对象。

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
public VbaModule get(int index)
```


通过索引获取列表中的 [VbaModule](../../com.aspose.cells/vbamodule)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
### get(String name) {#get-java.lang.String-}
```
public VbaModule get(String name)
```


通过名称获取列表中的 [VbaModule](../../com.aspose.cells/vbamodule)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 模块的名称。 |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
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
### getDesignerStorage(String name) {#getDesignerStorage-java.lang.String-}
```
public byte[] getDesignerStorage(String name)
```


表示设计器的数据。

**Remarks**

我们不支持解析它们。仅用于复制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
byte[]
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




### remove(Worksheet sheet) {#remove-com.aspose.cells.Worksheet-}
```
public void remove(Worksheet sheet)
```


删除工作表的模块。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | 工作表 |

### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


通过名称删除模块

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除指定索引处的项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除的项的零基索引。 |

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

