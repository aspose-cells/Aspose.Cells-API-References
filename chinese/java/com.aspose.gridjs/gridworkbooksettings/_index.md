---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作簿的设置。"
type: docs
url: /zh/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

表示工作簿的设置。

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | 获取文件的作者。 |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | 指示在设置 Style.Custom 时是否检查自定义数字格式，默认值为 false。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | 指示是否创建计算公式链。 |
| [getDate1904()](#getDate1904--) | 获取一个值，表示工作簿是否使用 1904 日期系统。 |
| [getEnableMacros()](#getEnableMacros--) | 启用宏；目前仅在将工作表复制到同一本工作簿的另一个工作表时有效。 |
| [getForceFullCalculate()](#getForceFullCalculate--) | 指示在触发计算时是否每次完全计算。 |
| [getIteration()](#getIteration--) | 指示是否使用迭代来解决循环引用。 |
| [getMaxIteration()](#getMaxIteration--) | 返回或设置解决循环引用的最大迭代次数，默认值为 100。 |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | 如果此工作簿中的计算仅使用显示的数字精度，则为 true。 |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | 指示是否在打开文件时重新计算所有公式。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 设置文件的作者。 |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | 指示在设置 Style.Custom 时是否检查自定义数字格式，默认值为 false。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | 指示是否创建计算公式链。 |
| [setDate1904(boolean value)](#setDate1904-boolean-) | 设置表示工作簿是否使用 1904 日期系统的值。 |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | 启用宏；目前仅在将工作表复制到同一本工作簿的另一个工作表时有效。 |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | 指示在触发计算时是否每次完全计算。 |
| [setIteration(boolean value)](#setIteration-boolean-) | 指示是否使用迭代来解决循环引用。 |
| [setMaxIteration(int value)](#setMaxIteration-int-) | 返回或设置解决循环引用的最大迭代次数，默认值为 100。 |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | 如果此工作簿中的计算仅使用显示的数字精度，则为 true。 |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | 指示是否在打开文件时重新计算所有公式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


获取文件的作者。

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


指示在设置 Style.Custom 时是否检查自定义数字格式，默认值为 false。

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


在用户修改单元格相关对象时是否检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，则会抛出异常。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置的值对 Excel 文件格式无效，则后续不应将工作簿另存为 Excel 文件格式。否则生成的 Excel 文件可能出现意外错误。默认值为 false。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


指示是否创建计算公式链。默认值为 false。

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


获取一个值，表示工作簿是否使用 1904 日期系统。

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


启用宏；目前仅在将工作表复制到同一本工作簿的另一个工作表时有效。

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


指示在触发计算时是否每次完全计算。

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


指示是否使用迭代来解决循环引用。

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


返回或设置解决循环引用的最大迭代次数，默认值为 100。

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


如果此工作簿中的计算仅使用显示的数字精度，则为 true。

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


指示是否在打开文件时重新计算所有公式。默认值为 true。

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


设置文件的作者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


指示在设置 Style.Custom 时是否检查自定义数字格式，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


在用户修改单元格相关对象时是否检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，则会抛出异常。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置的值对 Excel 文件格式无效，则后续不应将工作簿另存为 Excel 文件格式。否则生成的 Excel 文件可能出现意外错误。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


指示是否创建计算公式链。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


设置表示工作簿是否使用 1904 日期系统的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


启用宏；目前仅在将工作表复制到同一本工作簿的另一个工作表时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


指示在触发计算时是否每次完全计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


指示是否使用迭代来解决循环引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


返回或设置解决循环引用的最大迭代次数，默认值为 100。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


如果此工作簿中的计算仅使用显示的数字精度，则为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


指示是否在打开文件时重新计算所有公式。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

