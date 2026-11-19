---
title: "CellsDataTableFactory"
second_title: "Aspose.Cells for Java API 参考"
description: "用于从自定义对象构建 ICellsDataTable 的实用工具，方便用户使用。"
type: docs
url: /zh/java/com.aspose.cells/cellsdatatablefactory/
---

**Inheritance:**
java.lang.Object
```
public class CellsDataTableFactory
```

用于从自定义对象构建 ICellsDataTable 的实用工具，方便用户。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getInstance(double[] vals, boolean vertial)](#getInstance-double---boolean-) | 从给定的 double 值序列创建 ICellsDataTable。 |
| [getInstance(double[] vals, String[] columnNames)](#getInstance-double---java.lang.String---) | 从给定的 double 值序列创建 ICellsDataTable。 |
| [getInstance(double[][] vals)](#getInstance-double-----) | 从给定的二维数组创建 ICellsDataTable。 |
| [getInstance(int[] vals, boolean vertial)](#getInstance-int---boolean-) | 从给定的整数值序列创建 ICellsDataTable。 |
| [getInstance(int[] vals, String[] columnNames)](#getInstance-int---java.lang.String---) | 从给定的整数值序列创建 ICellsDataTable。 |
| [getInstance(int[][] vals)](#getInstance-int-----) | 从给定的二维数组创建 ICellsDataTable。 |
| [getInstance(Object[] vals, boolean vertial)](#getInstance-java.lang.Object---boolean-) | 从给定的对象序列创建 ICellsDataTable。 |
| [getInstance(Object[] vals, String[] columnNames)](#getInstance-java.lang.Object---java.lang.String---) | 从给定的对象序列创建 ICellsDataTable。 |
| [getInstance(Object[][] vals)](#getInstance-java.lang.Object-----) | 从给定的二维数组创建 ICellsDataTable。 |
| [getInstance(Object[][] vals, boolean hasHeader, String[] columnNames)](#getInstance-java.lang.Object-----boolean-java.lang.String---) | 从给定的对象序列创建 ICellsDataTable。 |
| [getInstance(Collection collection)](#getInstance-java.util.Collection-) | 从给定的集合创建 ICellsDataTable。 |
| [getInstance(Collection collection, boolean hasHeader)](#getInstance-java.util.Collection-boolean-) | 从给定的集合创建 ICellsDataTable。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getInstance(double[] vals, boolean vertial) {#getInstance-double---boolean-}
```
public ICellsDataTable getInstance(double[] vals, boolean vertial)
```


从给定的 double 值序列创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | double[] | 用于构建表的 double 值 |
| vertial | boolean | 是否按 double 值垂直（true）或水平（false）构建表格 |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(double[] vals, String[] columnNames) {#getInstance-double---java.lang.String---}
```
public ICellsDataTable getInstance(double[] vals, String[] columnNames)
```


从给定的 double 值序列创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | double[] | 用于构建表的 double 值 |
| columnNames | java.lang.String[] | 表格的列名。其长度只能是 1（通过 double values 垂直构建表格）或 double values 的长度（通过 double values 水平构建表格） |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(double[][] vals) {#getInstance-double-----}
```
public ICellsDataTable getInstance(double[][] vals)
```


从给定的二维数组创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | double[][] | 用于构建表的 double 值 |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[] vals, boolean vertial) {#getInstance-int---boolean-}
```
public ICellsDataTable getInstance(int[] vals, boolean vertial)
```


从给定的整数值序列创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | int[] | 用于构建表格的 int values |
| vertial | boolean | 是否通过 int values 垂直构建表格（true）或水平构建表格（false） |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[] vals, String[] columnNames) {#getInstance-int---java.lang.String---}
```
public ICellsDataTable getInstance(int[] vals, String[] columnNames)
```


从给定的整数值序列创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | int[] | 用于构建表格的 int values |
| columnNames | java.lang.String[] | 表格的列名。其长度只能是 1（通过 int values 垂直构建表格）或 int values 的长度（通过 int values 水平构建表格） |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[][] vals) {#getInstance-int-----}
```
public ICellsDataTable getInstance(int[][] vals)
```


从给定的二维数组创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | int[][] | 用于构建表格的 int values |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[] vals, boolean vertial) {#getInstance-java.lang.Object---boolean-}
```
public ICellsDataTable getInstance(Object[] vals, boolean vertial)
```


从给定的对象序列创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | java.lang.Object[] | 用于构建表格的 objects |
| vertial | boolean | 是否通过 objects 垂直构建表格（true）或水平构建表格（false） |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[] vals, String[] columnNames) {#getInstance-java.lang.Object---java.lang.String---}
```
public ICellsDataTable getInstance(Object[] vals, String[] columnNames)
```


从给定的对象序列创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | java.lang.Object[] | 用于构建表格的 objects |
| columnNames | java.lang.String[] | 表格的列名。其长度只能是 1（通过 objects 垂直构建表格）或 objects 的长度（通过 objects 水平构建表格） |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[][] vals) {#getInstance-java.lang.Object-----}
```
public ICellsDataTable getInstance(Object[][] vals)
```


从给定的二维数组创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | java.lang.Object[][] | 用于构建表格的 objects |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[][] vals, boolean hasHeader, String[] columnNames) {#getInstance-java.lang.Object-----boolean-java.lang.String---}
```
public ICellsDataTable getInstance(Object[][] vals, boolean hasHeader, String[] columnNames)
```


从给定的对象序列创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| vals | java.lang.Object[][] | 用于构建表格的 objects |
| hasHeader | boolean | 指示第一行是否为标题行。 |
| columnNames | java.lang.String[] | 表格的列名。其长度只能是 1（通过 objects 垂直构建表格）或 objects 的长度（通过 objects 水平构建表格） |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Collection collection) {#getInstance-java.util.Collection-}
```
public ICellsDataTable getInstance(Collection collection)
```


从给定的集合创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| collection | java.util.Collection | 用于构建表格的 collection |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Collection collection, boolean hasHeader) {#getInstance-java.util.Collection-boolean-}
```
public ICellsDataTable getInstance(Collection collection, boolean hasHeader)
```


从给定的集合创建 ICellsDataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| collection | java.util.Collection | 用于构建表格的 collection |
| hasHeader | boolean | 指示第一行是否为标题 |

**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
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

