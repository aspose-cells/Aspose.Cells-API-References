---
title: "CopyOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示复制选项。"
type: docs
url: /zh/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

表示复制选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions 构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | 指示是否以字符单位复制列宽。 |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | 如果公式对目标位置无效，则仅复制值。 |
| [getCopyNames()](#getCopyNames--) | 指示是否复制名称。 |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | 指示在将范围复制到相邻范围时是否扩展范围。 |
| [getKeepMacros()](#getKeepMacros--) | 指示是否保留宏； |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | 当在同一文件中复制范围且图表引用源工作表时，False 表示复制的图表的数据源不会被更改。 |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | 在 ms excel 中，当在复制工作表到另一个工作表时复制引用其他工作表的公式，复制的公式应引用源工作簿。 |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | 指示如果未复制被引用的工作表，是否引用目标工作表。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | 指示是否以字符单位复制列宽。 |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | 如果公式对目标位置无效，则仅复制值。 |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | 指示是否复制名称。 |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | 指示在将范围复制到相邻范围时是否扩展范围。 |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | 指示是否保留宏； |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | 当在同一文件中复制范围且图表引用源工作表时，False 表示复制的图表的数据源不会被更改。 |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | 在 ms excel 中，当在复制工作表到另一个工作表时复制引用其他工作表的公式，复制的公式应引用源工作簿。 |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | 指示如果未复制被引用的工作表，是否引用目标工作表。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


CopyOptions 构造函数。

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


指示是否以字符单位复制列宽。

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


如果公式对目标位置无效，则仅复制值。

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


指示是否复制名称。

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


指示在将范围复制到相邻范围时是否扩展范围。

**Remarks**

如果为 true，则仅扩展超链接的范围，在将超链接复制到相邻行时不添加新超链接。

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


指示是否保留宏；

**Remarks**

仅用于复制工作簿。

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


当在同一文件中复制范围且图表引用源工作表时，False 表示复制的图表的数据源不会被更改。True 表示复制的图表的数据源引用目标工作表。

**Remarks**

默认值为 false，行为与 MS Excel 相同。例如：如果将数据源为 \"sheet1!A1:B10\" 的图表从工作表 \"sheet1\" 复制到另一个工作表 \"sheet2\"，数据源将更改为 \"sheet2!A1:B10\"

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


在 ms excel 中，当在复制工作表到另一个工作表时复制引用其他工作表的公式，复制的公式应引用源工作簿。然而，在某些情况下用户可能需要复制的公式引用同一工作簿中同名的工作表，例如这些工作表在此复制操作之前已经被复制，则此属性应保持为 true。

**Remarks**

默认值为 true。

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


指示如果未复制被引用的工作表，是否引用目标工作表。

**Remarks**

仅在从另一本工作簿复制范围或工作表时有效。

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


指示是否以字符单位复制列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


如果公式对目标位置无效，则仅复制值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


指示是否复制名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


指示在将范围复制到相邻范围时是否扩展范围。

**Remarks**

如果为 true，则仅扩展超链接的范围，在将超链接复制到相邻行时不添加新超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


指示是否保留宏；

**Remarks**

仅用于复制工作簿。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


当在同一文件中复制范围且图表引用源工作表时，False 表示复制的图表的数据源不会被更改。True 表示复制的图表的数据源引用目标工作表。

**Remarks**

默认值为 false，行为与 MS Excel 相同。例如：如果将数据源为 \"sheet1!A1:B10\" 的图表从工作表 \"sheet1\" 复制到另一个工作表 \"sheet2\"，数据源将更改为 \"sheet2!A1:B10\"

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


在 ms excel 中，当在复制工作表到另一个工作表时复制引用其他工作表的公式，复制的公式应引用源工作簿。然而，在某些情况下用户可能需要复制的公式引用同一工作簿中同名的工作表，例如这些工作表在此复制操作之前已经被复制，则此属性应保持为 true。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


指示如果未复制被引用的工作表，是否引用目标工作表。

**Remarks**

仅在从另一本工作簿复制范围或工作表时有效。

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

