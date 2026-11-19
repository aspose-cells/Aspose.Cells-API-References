---
title: "LoadFilter"
second_title: "Aspose.Cells for Java API 参考"
description: "表示在从模板加载工作簿时提供加载数据选项的过滤器。"
type: docs
url: /zh/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

表示在从模板加载工作簿时提供加载数据选项的过滤器。

**Remarks**

用户可以指定过滤选项或实现自己的 LoadFilter 来指定如何加载数据。

**Example**

以下示例展示了如何根据工作表的属性确定过滤选项。

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | 使用默认过滤选项 LoadDataFilterOptions.All 构造一个 LoadFilter。 |
| [LoadFilter(int opts)](#LoadFilter-int-) | 使用给定的过滤选项构造一个 LoadFilter。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | 用于指示应加载哪些数据的过滤选项。 |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | 指定要加载的工作表（索引）及其顺序。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | 用于指示应加载哪些数据的过滤选项。 |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | 在加载给定工作表之前准备过滤选项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


使用默认过滤选项 LoadDataFilterOptions.All 构造一个 LoadFilter。

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


使用给定的过滤选项构造一个 LoadFilter。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions)。默认过滤选项 |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


用于指示应加载哪些数据的过滤选项。

参见 [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions)。

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


指定要加载的工作表（索引）及其顺序。默认值为 null，表示加载模板文件中按默认顺序的所有工作表。如果不为 null 且某些工作表的索引未出现在返回的数组中，则该工作表将不会被加载。

**Returns:**
int[]
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


用于指示应加载哪些数据的过滤选项。

参见 [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


在加载给定工作表之前准备过滤选项。用户对 LoadFilter 的实现可以在此更改 LoadDataFilterOptions，以指示如何为此工作表加载数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | 要加载的工作表。由于大多数数据和属性尚未加载，此处只能使用该工作表对象的少数属性。可用的属性有：Name、Index、VisibilityType。 |

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

