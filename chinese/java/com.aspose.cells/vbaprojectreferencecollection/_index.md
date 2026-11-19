---
title: "VbaProjectReferenceCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 VBA 项目的所有引用。"
type: docs
url: /zh/java/com.aspose.cells/vbaprojectreferencecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaProjectReferenceCollection extends CollectionBase
```

表示 VBA 项目的所有引用。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 添加对 twiddled 类型库及其扩展类型库的引用。 |
| [addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 添加对 twiddled 类型库及其扩展类型库的引用。 |
| [addProjectReferernce(String name, String absoluteLibid, String relativeLibid)](#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-) | 添加对外部 VBA 项目的引用。 |
| [addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)](#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-) | 添加对外部 VBA 项目的引用。 |
| [addRegisteredReference(String name, String libid)](#addRegisteredReference-java.lang.String-java.lang.String-) | 添加对 Automation 类型库的引用。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [copy(VbaProjectReferenceCollection source)](#copy-com.aspose.cells.VbaProjectReferenceCollection-) | 从其他 VBA 项目复制引用。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int i)](#get-int-) | 通过索引获取列表中的引用。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


添加对 twiddled 类型库及其扩展类型库的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 引用的名称。 |
| libid | java.lang.String | Automation 类型库的标识符。 |
| twiddledlibid | java.lang.String | twiddled 类型库的标识符 |
| extendedLibid | java.lang.String | 扩展类型库的标识符 |

**Returns:**
int -
### addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


添加对 twiddled 类型库及其扩展类型库的引用。

**Remarks**

注意：此方法已过时。请改用 VbaProjectReferenceCollection.AddControlReferernce() 方法。该方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 引用的名称。 |
| libid | java.lang.String | Automation 类型库的标识符。 |
| twiddledlibid | java.lang.String | twiddled 类型库的标识符 |
| extendedLibid | java.lang.String | 扩展类型库的标识符 |

**Returns:**
int -
### addProjectReferernce(String name, String absoluteLibid, String relativeLibid) {#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectReferernce(String name, String absoluteLibid, String relativeLibid)
```


添加对外部 VBA 项目的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 引用的名称。 |
| absoluteLibid | java.lang.String | 带有绝对路径的被引用 VBA 项目的标识符。 |
| relativeLibid | java.lang.String | 带有相对路径的被引用 VBA 项目的标识符。 |

**Returns:**
int -
### addProjectRefrernce(String name, String absoluteLibid, String relativeLibid) {#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)
```


添加对外部 VBA 项目的引用。

**Remarks**

注意：此方法已过时。请改用 VbaProjectReferenceCollection.AddProjectReferernce() 方法。该方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 引用的名称。 |
| absoluteLibid | java.lang.String | 带有绝对路径的被引用 VBA 项目的标识符。 |
| relativeLibid | java.lang.String | 带有相对路径的被引用 VBA 项目的标识符。 |

**Returns:**
int -
### addRegisteredReference(String name, String libid) {#addRegisteredReference-java.lang.String-java.lang.String-}
```
public int addRegisteredReference(String name, String libid)
```


添加对 Automation 类型库的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 引用的名称。 |
| libid | java.lang.String | Automation 类型库的标识符。 |

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
### copy(VbaProjectReferenceCollection source) {#copy-com.aspose.cells.VbaProjectReferenceCollection-}
```
public void copy(VbaProjectReferenceCollection source)
```


从其他 VBA 项目复制引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection) | 源引用。 |

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
### get(int i) {#get-int-}
```
public VbaProjectReference get(int i)
```


通过索引获取列表中的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| i | int | 索引。 |

**Returns:**
[VbaProjectReference](../../com.aspose.cells/vbaprojectreference) - 
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

