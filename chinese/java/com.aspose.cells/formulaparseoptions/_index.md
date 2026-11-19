---
title: "FormulaParseOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示解析公式时的选项。"
type: docs
url: /zh/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

表示解析公式时的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | 是否在当前工作簿的现有外部链接中检查用户自定义函数的加载项（无外部链接）。 |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | 自定义函数解析的定义。 |
| [getLocaleDependent()](#getLocaleDependent--) | 公式是否已本地化格式化。 |
| [getParse()](#getParse--) | 是否解析给定的公式。 |
| [getR1C1Style()](#getR1C1Style--) | 公式是否为 R1C1 引用样式。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | 是否在当前工作簿的现有外部链接中检查用户自定义函数的加载项（无外部链接）。 |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | 自定义函数解析的定义。 |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | 公式是否已本地化格式化。 |
| [setParse(boolean value)](#setParse-boolean-) | 是否解析给定的公式。 |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | 公式是否为 R1C1 引用样式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


是否在当前工作簿的现有外部链接中检查用户自定义函数的加载项（无外部链接）。默认值为 true（如果用户自定义函数匹配现有外部链接中的某个加载项，则视为该加载项）。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


自定义函数解析的定义。

**Remarks**

对于某些特殊需求，例如在用户自定义引擎中计算自定义函数时，需要以数组模式计算其某些参数，使用此属性可以在解析公式时将这些参数标记为数组模式。否则用户需要稍后通过 [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) 更新这些自定义函数以获得相同的结果。

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


公式是否使用本地化格式。默认值为 false。

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


是否解析给定的公式。默认值为 true。如果为 false，则给定的公式字符串将保持原样，直到用户调用其他方法进行解析，或其他操作（如计算公式）需要解析后的公式数据。

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


公式是否为 R1C1 引用样式。默认值为 false。

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




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


是否在当前工作簿的现有外部链接中检查用户自定义函数的加载项（无外部链接）。默认值为 true（如果用户自定义函数匹配现有外部链接中的某个加载项，则视为该加载项）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


自定义函数解析的定义。

**Remarks**

对于某些特殊需求，例如在用户自定义引擎中计算自定义函数时，需要以数组模式计算其某些参数，使用此属性可以在解析公式时将这些参数标记为数组模式。否则用户需要稍后通过 [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) 更新这些自定义函数以获得相同的结果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


公式是否使用本地化格式。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


是否解析给定的公式。默认值为 true。如果为 false，则给定的公式字符串将保持原样，直到用户调用其他方法进行解析，或其他操作（如计算公式）需要解析后的公式数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


公式是否为 R1C1 引用样式。默认值为 false。

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

