---
title: "RowCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "收集表示工作表中各个行的对象。"
type: docs
url: /zh/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

收集 [Row](../../com.aspose.cells/row) 对象，这些对象表示工作表中各个行。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [clear()](#clear--) | 清除所有行和单元格。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | 通过给定的行索引获取一个 [Row](../../com.aspose.cells/row) 对象。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取此集合中行的数量。 |
| [getRowByIndex(int index)](#getRowByIndex-int-) | 通过列表中的位置获取行对象。 |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | 获取一个遍历此集合中行的枚举器。 |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | 获取一个遍历此集合中行的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除此集合中指定索引（位置）的行项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


清除所有行和单元格。

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


通过给定的行索引获取一个 [Row](../../com.aspose.cells/row) 对象。如果给定行索引的 Row 对象之前不存在，将会实例化它。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


获取此集合中行的数量。

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


通过列表中的位置获取行对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 位置。 |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
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


获取一个遍历此集合中行的枚举器。

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - 将遍历此集合中所有现有行的行枚举器。
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


获取一个遍历此集合中行的枚举器。

**Remarks**

如果在使用枚举器遍历期间，行集合会被修改（通过可能导致实例化新 Row 或删除现有 Row 的操作），则应使用同步枚举器而不是普通枚举器，以便遍历能够从上一次 MoveNext() 所遍历位置的下一个位置继续。虽然同步枚举器的优势在于不会跳过或重复遍历元素，但其缺点是与普通枚举器相比，性能会略有下降。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 反向 | boolean | 是否以反向顺序枚举行。 |
| 同步 | boolean | 返回的枚举器是否应检查行集合的修改并保持与之同步。 |

**Returns:**
java.util.Iterator - 将遍历此集合中所有现有行的行枚举器。
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


移除此集合中指定索引（位置）的行项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 零基索引（位置，不是 [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)）在此集合中现有的行项。 |

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

