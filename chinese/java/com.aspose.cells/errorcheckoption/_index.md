---
title: "ErrorCheckOption"
second_title: "Aspose.Cells for Java API 参考"
description: "对特定范围应用的错误检查设置。"
type: docs
url: /zh/java/com.aspose.cells/errorcheckoption/
---

**Inheritance:**
java.lang.Object
```
public class ErrorCheckOption
```

对特定范围应用的错误检查设置。

**Example**

```
           Workbook workbook = new Workbook();
           ErrorCheckOptionCollection opts = workbook.getWorksheets().get(0).getErrorCheckOptions();
           int optionIdx = opts.add();
           ErrorCheckOption opt = opts.get(optionIdx);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_FORMULA, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_RANGE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_DATE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_NUMBER, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.VALIDATION, false);
           opt.addRange(CellArea.createCellArea("A1", "B10"));
           workbook.save("Book1.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addRange(CellArea ca)](#addRange-com.aspose.cells.CellArea-) | 通过此设置添加一个受影响的范围。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCountOfRange()](#getCountOfRange--) | 获取此设置影响的范围数量。 |
| [getRange(int index)](#getRange-int-) | 根据给定索引获取此设置的受影响范围。 |
| [hashCode()](#hashCode--) |  |
| [isErrorCheck(int errorCheckType)](#isErrorCheck-int-) | 检查给定的错误类型是否会被检查。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeRange(int index)](#removeRange-int-) | 根据给定索引移除一个范围。 |
| [setErrorCheck(int errorCheckType, boolean isCheck)](#setErrorCheck-int-boolean-) | 设置是否检查给定的错误类型。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(CellArea ca) {#addRange-com.aspose.cells.CellArea-}
```
public int addRange(CellArea ca)
```


通过此设置添加一个受影响的范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 要添加的范围。 |

**Returns:**
int - 此设置的范围列表中已添加范围的索引。
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
### getCountOfRange() {#getCountOfRange--}
```
public int getCountOfRange()
```


获取此设置影响的范围数量。

**Returns:**
int - 此设置影响的范围数量。
### getRange(int index) {#getRange-int-}
```
public CellArea getRange(int index)
```


根据给定索引获取此设置的受影响范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 范围的索引 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - return influenced range at given index.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isErrorCheck(int errorCheckType) {#isErrorCheck-int-}
```
public boolean isErrorCheck(int errorCheckType)
```


检查给定的错误类型是否会被检查。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). 可检查的错误类型 |

**Returns:**
boolean - 如果给定错误类型将被检查则返回 true（如果检查失败，单元格将显示绿色三角形）。
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeRange(int index) {#removeRange-int-}
```
public void removeRange(int index)
```


根据给定索引移除一个范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除的范围的索引。 |

### setErrorCheck(int errorCheckType, boolean isCheck) {#setErrorCheck-int-boolean-}
```
public void setErrorCheck(int errorCheckType, boolean isCheck)
```


设置是否检查给定的错误类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). 可检查的错误类型。 |
| isCheck | boolean | 如果需要检查给定的错误类型，则为 true（如果检查失败，单元格将显示绿色三角形）。 |

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

