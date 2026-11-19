---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作簿的设置。"
type: docs
url: /zh/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

表示工作簿的设置。

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | 默认构造函数 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | 获取文件的作者。 |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | 获取在设置 Style.Custom 时是否检查自定义数字格式。 |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | 获取是否创建已计算公式链。 |
| [getDate1904()](#getDate1904--) | 获取表示工作簿是否使用 1904 日期系统的值。 |
| [getEnableMacros()](#getEnableMacros--) | 获取是否启用宏；目前仅在将工作表复制到同一工作簿的其他工作表时有效。 |
| [getForceFullCalculate()](#getForceFullCalculate--) | 获取是否在每次触发计算时完全重新计算。 |
| [getIteration()](#getIteration--) | 获取是否使用迭代来解决循环引用。 |
| [getMaxIteration()](#getMaxIteration--) | 获取解决循环引用的最大迭代次数，默认值为 100。 |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | 如果此工作簿中的计算仅使用显示的数字精度，则为 true。 |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | 获取是否在打开文件时重新计算所有公式。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 设置文件的作者。 |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | 设置在设置 Style.Custom 时是否检查自定义数字格式。 |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | 设置是否创建已计算公式链。 |
| [setDate1904(boolean value)](#setDate1904-boolean-) | 设置表示工作簿是否使用 1904 日期系统的值。 |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | 设置是否启用宏；目前仅在将工作表复制到同一工作簿的其他工作表时有效。 |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | 设置是否在每次触发计算时完全重新计算。 |
| [setIteration(boolean value)](#setIteration-boolean-) | 设置是否使用迭代来解决循环引用。 |
| [setMaxIteration(int value)](#setMaxIteration-int-) | 设置解决循环引用的最大迭代次数，默认值为 100。 |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | 如果此工作簿中的计算仅使用显示的数字精度，则为 true。 |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | 设置是否在打开文件时重新计算所有公式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


默认构造函数

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


获取在设置 Style.Custom 时是否检查自定义数字格式。

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


获取是否创建计算公式链。默认值为 false。

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


获取表示工作簿是否使用 1904 日期系统的值。

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


获取是否启用宏；目前仅在将工作表复制到同一工作簿的其他工作表时有效。

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


获取是否在每次触发计算时完全重新计算。

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


获取是否使用迭代来解决循环引用。

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


获取解决循环引用的最大迭代次数，默认值为 100。

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


如果此工作簿中的计算仅使用显示的数字精度，则为 true。

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。

**Remarks**

通常这些空格和换行符仅用于视觉效果，是否保留它们并不影响计算结果。出于性能考虑，如果没有特殊需求，处理公式时最好不要保留它们。

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


获取是否在打开文件时重新计算所有公式。

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


设置在设置 Style.Custom 时是否检查自定义数字格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


设置是否创建计算公式链。默认值为 false。

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


设置是否启用宏；目前仅在将工作表复制到同一工作簿的其他工作表时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


设置是否在每次触发计算时完全重新计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


设置是否使用迭代来解决循环引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


设置解决循环引用的最大迭代次数，默认值为 100。

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

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。

**Remarks**

通常这些空格和换行符仅用于视觉效果，是否保留它们并不影响计算结果。出于性能考虑，如果没有特殊需求，处理公式时最好不要保留它们。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


设置是否在打开文件时重新计算所有公式。

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

