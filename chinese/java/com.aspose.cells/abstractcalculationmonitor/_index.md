---
title: "AbstractCalculationMonitor"
second_title: "Aspose.Cells for Java API 参考"
description: "为用户提供监视，以跟踪公式计算的进度。"
type: docs
url: /zh/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

为用户提供监视，以跟踪公式计算的进度。

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | 在单元格计算完成后实现此方法以进行业务处理。 |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | 在计算单元格之前实现此方法以进行业务处理。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | 获取单元格新计算的值。 |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | 获取已计算单元格的旧值。 |
| [getValueChanged()](#getValueChanged--) | 计算后单元格的值是否已更改。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | 在计算具有循环引用的公式时实现此方法以进行业务处理。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


在单元格计算完成后实现此方法以进行业务处理。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 单元格所属工作表的索引。 |
| rowIndex | int | 单元格的行索引 |
| colIndex | int | 单元格的列索引 |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


在计算单元格之前实现此方法以进行业务处理。

**Remarks**

对于数组公式中的单元格，此方法可能不会被执行，因为这些单元格通常会一起计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 单元格所属工作表的索引。 |
| rowIndex | int | 单元格的行索引 |
| colIndex | int | 单元格的列索引 |

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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


获取单元格的新计算值。应仅在 [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) 中使用。

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


获取已计算单元格的旧值。应仅在 [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) 和 [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) 中使用。

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


指示单元格的值在计算后是否已更改。应仅在 [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) 中使用。

**Returns:**
boolean
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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


在计算具有循环引用的公式时实现此方法以进行业务处理。

**Remarks**

在实现中，用户也可以将预期值设置为这些单元格的部分或全部计算结果，以便公式引擎不会递归计算它们。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator 包含表示依赖循环引用的单元格的 [CalculationCell](../../com.aspose.cells/calculationcell) 项。 |

**Returns:**
boolean - 此调用后公式引擎是否需要循环计算这些单元格。True 表示让公式引擎继续对其进行计算。False 表示让公式引擎仅将这些单元格标记为已计算。
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

