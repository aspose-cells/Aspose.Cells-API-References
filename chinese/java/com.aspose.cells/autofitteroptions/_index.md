---
title: "AutoFitterOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示所有自动适配选项。"
type: docs
url: /zh/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

表示所有自动适配选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | 指示在行中合并单元格时是否自动适配行高。 |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | 获取合并单元格的自动适配行高类型。 |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | 获取自动换行文本的类型。 |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | 获取默认编辑语言。 |
| [getForRendering()](#getForRendering--) | 指示是否为渲染目的进行适配。 |
| [getFormatStrategy()](#getFormatStrategy--) | 获取格式化策略。 |
| [getIgnoreHidden()](#getIgnoreHidden--) | 忽略隐藏的行/列。 |
| [getMaxRowHeight()](#getMaxRowHeight--) | 在自动适配行时获取最大行高（单位为 Point）。 |
| [getOnlyAuto()](#getOnlyAuto--) | 指示是否仅适配高度未自定义的行。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | 指示在行中合并单元格时是否自动适配行高。 |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | 设置合并单元格的自动适配行高类型。 |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | 设置自动换行文本的类型。 |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | 设置默认编辑语言。 |
| [setForRendering(boolean value)](#setForRendering-boolean-) | 指示是否为渲染目的进行适配。 |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | 设置格式化策略。 |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | 忽略隐藏的行/列。 |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | 在自动适配行时设置最大行高（单位为 Point）。 |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | 指示是否仅适配高度未自定义的行。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


指示在行中合并单元格时是否自动适配行高。默认值为 false。

**Remarks**

注意：此成员现已过时。请改用 AutoFitterOptions.AutoFitMergedCellsType 属性。该属性将在自 2018 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


获取合并单元格的自动适配行高类型。

参见 [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype)。

**Remarks**

Excel 在调整行高时默认忽略合并单元格，因此 Aspose.Cells 与 MS Excel 的默认行为一致。请设置此类型以更改合并单元格自动适应行高的方式。

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


获取自动换行文本的类型。

参见 [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype)。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


获取默认编辑语言。

参见 [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage)。

**Remarks**

当设置不同的编辑语言时，可能会显示/渲染文本段落的不同布局。默认值为 [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO)。

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


指示是否为渲染目的进行适配。

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


获取格式化策略。

参见 [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy)。

**Remarks**

默认值为 CellStyle，以提升性能。

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


忽略隐藏的行/列。

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


在自动适配行时获取最大行高（单位为 Point）。

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


指示是否仅适配高度未自定义的行。

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


指示在行中合并单元格时是否自动适配行高。默认值为 false。

**Remarks**

注意：此成员现已过时。请改用 AutoFitterOptions.AutoFitMergedCellsType 属性。该属性将在自 2018 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


设置合并单元格的自动适配行高类型。

参见 [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype)。

**Remarks**

Excel 在调整行高时默认忽略合并单元格，因此 Aspose.Cells 与 MS Excel 的默认行为一致。请设置此类型以更改合并单元格自动适应行高的方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


设置自动换行文本的类型。

参见 [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


设置默认编辑语言。

参见 [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage)。

**Remarks**

当设置不同的编辑语言时，可能会显示/渲染文本段落的不同布局。默认值为 [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


指示是否为渲染目的进行适配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


设置格式化策略。

参见 [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy)。

**Remarks**

默认值为 CellStyle，以提升性能。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


忽略隐藏的行/列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


在自动适配行时设置最大行高（单位为 Point）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


指示是否仅适配高度未自定义的行。

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

