---
title: "ListColumn"
second_title: "Aspose.Cells for Java API 参考"
description: "表示表格中的列。"
type: docs
url: /zh/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

表示表格中的列。

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | 获取此列表列的公式。 |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | 获取此列表列的合计行公式。 |
| [getDataStyle()](#getDataStyle--) | 获取表中此列数据的样式。 |
| [getFormula()](#getFormula--) | 获取列表列的公式。 |
| [getName()](#getName--) | 获取列的名称。 |
| [getRange()](#getRange--) | 获取此列表列的范围。 |
| [getTotalsCalculation()](#getTotalsCalculation--) | 获取列表列的汇总行中的计算类型。 |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | 获取汇总行的显示标签。 |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | 指示公式是否为数组公式。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | 设置此列表列的公式。 |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | 获取此列表列的合计行公式。 |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | 设置表中此列数据的样式。 |
| [setFormula(String value)](#setFormula-java.lang.String-) | 设置列表列的公式。 |
| [setName(String value)](#setName-java.lang.String-) | 设置列的名称。 |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | 设置列表列的汇总行中的计算类型。 |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | 设置汇总行的显示标签。 |
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
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


获取此列表列的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 此列表列的公式。
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


获取此列表列的合计行公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 此列表列的公式。
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


获取表中此列数据的样式。

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


获取列表列的公式。

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


获取列的名称。

**Remarks**

如果设置列的名称，相应单元格的值也会被更改。

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


获取此列表列的范围。

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


获取列表列的汇总行中的计算类型。

参见 [TotalsCalculation](../../com.aspose.cells/totalscalculation)。

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


获取汇总行的显示标签。

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


指示公式是否为数组公式。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


设置此列表列的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 此列表列的公式。 |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


获取此列表列的合计行公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 此列表列的公式。 |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


设置表中此列数据的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


设置列表列的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置列的名称。

**Remarks**

如果设置列的名称，相应单元格的值也会被更改。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


设置列表列的汇总行中的计算类型。

参见 [TotalsCalculation](../../com.aspose.cells/totalscalculation)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


设置汇总行的显示标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

