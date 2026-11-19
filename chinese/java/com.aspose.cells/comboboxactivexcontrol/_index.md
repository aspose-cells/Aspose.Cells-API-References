---
title: "ComboBoxActiveXControl"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 ComboBox ActiveX 控件。"
type: docs
url: /zh/java/com.aspose.cells/comboboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ComboBoxActiveXControl extends ActiveXControl
```

表示 ComboBox ActiveX 控件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | 获取背景的 ole 颜色。 |
| [getBorderOleColor()](#getBorderOleColor--) | 获取背景的 ole 颜色。 |
| [getBorderStyle()](#getBorderStyle--) | 获取控件使用的边框类型。 |
| [getBoundColumn()](#getBoundColumn--) | 表示在 MultiSelect 属性值为 (fmMultiSelectSingle) 时，ComboBox 或 ListBox 的 Value 属性的确定方式。 |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | 表示在 ComboBox 或 ListBox 中显示的列数。 |
| [getColumnWidths()](#getColumnWidths--) | 获取列的宽度。 |
| [getData()](#getData--) | 获取控件的二进制数据。 |
| [getDropButtonStyle()](#getDropButtonStyle--) | 指定下拉按钮上显示的符号 |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | 指定进入控件时的选择行为。 |
| [getFont()](#getFont--) | 表示控件的字体。 |
| [getForeOleColor()](#getForeOleColor--) | 获取前景的 OLE 颜色。 |
| [getHeight()](#getHeight--) | 获取控件的高度（单位为点）。 |
| [getHideSelection()](#getHideSelection--) | 指示当控件未获得焦点时，控件中的选中文本是否显示为高亮。 |
| [getIMEMode()](#getIMEMode--) | 获取控件获得焦点时输入法编辑器的默认运行模式。 |
| [getLinkedCell()](#getLinkedCell--) | 获取链接的单元格。 |
| [getListFillRange()](#getListFillRange--) | 获取列表填充范围。 |
| [getListRows()](#getListRows--) | 表示列表中要显示的最大行数。 |
| [getListStyle()](#getListStyle--) | 获取视觉外观。 |
| [getListWidth()](#getListWidth--) | 获取宽度（单位为点）。 |
| [getMatchEntry()](#getMatchEntry--) | 指示 ListBox 或 ComboBox 在用户输入时如何搜索其列表。 |
| [getMaxLength()](#getMaxLength--) | 获取最大字符数 |
| [getMouseIcon()](#getMouseIcon--) | 获取用于在控件上显示为鼠标指针的自定义图标。 |
| [getMousePointer()](#getMousePointer--) | 获取在控件上显示为鼠标指针的图标类型。 |
| [getSelectionMargin()](#getSelectionMargin--) | 指示用户是否可以通过单击文本左侧区域来选择一行文本。 |
| [getShadow()](#getShadow--) | 指示是否显示阴影。 |
| [getShowColumnHeads()](#getShowColumnHeads--) | 指示是否显示列标题。 |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | 指定下拉按钮上显示的符号 |
| [getSpecialEffect()](#getSpecialEffect--) | 获取控件的特殊效果。 |
| [getTextAlign()](#getTextAlign--) | 表示控件使用的文本对齐方式。 |
| [getTextColumn()](#getTextColumn--) | 表示在 ComboBox 或 ListBox 中向用户显示的列。 |
| [getType()](#getType--) | 获取 ActiveX 控件的类型。 |
| [getValue()](#getValue--) | 获取控件的值。 |
| [getWidth()](#getWidth--) | 获取控件的宽度（单位为点）。 |
| [getWorkbook()](#getWorkbook--) | 获取 [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) 对象。 |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [isAutoWordSelected()](#isAutoWordSelected--) | 指定用于扩展选择的基本单位。 |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | 指示是否已为控件启用拖放功能。 |
| [isEditable()](#isEditable--) | 指示用户是否可以在控件中输入。 |
| [isEnabled()](#isEnabled--) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [isLocked()](#isLocked--) | 指示控件中的数据是否被锁定，无法编辑。 |
| [isTransparent()](#isTransparent--) | 指示控件是否透明。 |
| [isVisible()](#isVisible--) | 指示此控件是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | 指定用于扩展选择的基本单位。 |
| [setBackOleColor(int value)](#setBackOleColor-int-) | 设置背景的 OLE 颜色。 |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | 设置背景的 OLE 颜色。 |
| [setBorderStyle(int value)](#setBorderStyle-int-) | 设置控件使用的边框类型。 |
| [setBoundColumn(int value)](#setBoundColumn-int-) | 表示在 MultiSelect 属性值为 (fmMultiSelectSingle) 时，ComboBox 或 ListBox 的 Value 属性的确定方式。 |
| [setColumnCount(int value)](#setColumnCount-int-) | 表示在 ComboBox 或 ListBox 中显示的列数。 |
| [setColumnWidths(double value)](#setColumnWidths-double-) | 设置列的宽度。 |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | 指示是否已为控件启用拖放功能。 |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | 指定下拉按钮上显示的符号 |
| [setEditable(boolean value)](#setEditable-boolean-) | 指示用户是否可以在控件中输入。 |
| [setEnabled(boolean value)](#setEnabled-boolean-) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | 指定进入控件时的选择行为。 |
| [setForeOleColor(int value)](#setForeOleColor-int-) | 设置前景的 OLE 颜色。 |
| [setHeight(double value)](#setHeight-double-) | 设置控件的高度（单位为点）。 |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | 指示当控件未获得焦点时，控件中的选中文本是否显示为高亮。 |
| [setIMEMode(int value)](#setIMEMode-int-) | 设置控件获取焦点时输入法编辑器的默认运行模式。 |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | 设置链接的单元格。 |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | 设置列表填充范围。 |
| [setListRows(int value)](#setListRows-int-) | 表示列表中要显示的最大行数。 |
| [setListStyle(int value)](#setListStyle-int-) | 设置视觉外观。 |
| [setListWidth(double value)](#setListWidth-double-) | 设置宽度（单位为点）。 |
| [setLocked(boolean value)](#setLocked-boolean-) | 指示控件中的数据是否被锁定，无法编辑。 |
| [setMatchEntry(int value)](#setMatchEntry-int-) | 指示 ListBox 或 ComboBox 在用户输入时如何搜索其列表。 |
| [setMaxLength(int value)](#setMaxLength-int-) | 设置最大字符数 |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | 设置自定义图标，以在控件上显示为鼠标指针。 |
| [setMousePointer(int value)](#setMousePointer-int-) | 设置在控件上显示为鼠标指针的图标类型。 |
| [setSelectionMargin(boolean value)](#setSelectionMargin-boolean-) | 指示用户是否可以通过单击文本左侧区域来选择一行文本。 |
| [setShadow(boolean value)](#setShadow-boolean-) | 指示是否显示阴影。 |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | 指示是否显示列标题。 |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | 指定下拉按钮上显示的符号 |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | 设置控件的特殊效果。 |
| [setTextAlign(int value)](#setTextAlign-int-) | 表示控件使用的文本对齐方式。 |
| [setTextColumn(int value)](#setTextColumn-int-) | 表示在 ComboBox 或 ListBox 中向用户显示的列。 |
| [setTransparent(boolean value)](#setTransparent-boolean-) | 指示控件是否透明。 |
| [setValue(String value)](#setValue-java.lang.String-) | 设置控件的值。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示此控件是否可见。 |
| [setWidth(double value)](#setWidth-double-) | 以点为单位设置控件的宽度。 |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


获取背景的 ole 颜色。

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


获取背景的 ole 颜色。

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


获取控件使用的边框类型。

参见 [ControlBorderType](../../com.aspose.cells/controlbordertype)。

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


表示在 MultiSelect 属性值为 (fmMultiSelectSingle) 时，ComboBox 或 ListBox 的 Value 属性的确定方式。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


表示在 ComboBox 或 ListBox 中显示的列数。

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


获取列的宽度。

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


获取控件的二进制数据。

**Returns:**
byte[]
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


指定下拉按钮上显示的符号

参见 [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle)。

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


指定进入控件时的选择行为。True 表示选择保持自上次控件处于活动状态时的状态不变。False 表示进入控件时将选中控件中的所有文本。

**Returns:**
boolean
### getFont() {#getFont--}
```
public Font getFont()
```


表示控件的字体。

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


获取前景的 OLE 颜色。

**Remarks**

不适用于 Image 控件。

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


获取控件的高度（单位为点）。

**Returns:**
double
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


指示当控件未获得焦点时，控件中的选中文本是否显示为高亮。

**Returns:**
boolean
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


获取控件获得焦点时输入法编辑器的默认运行模式。

参见 [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode)。

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


获取链接的单元格。

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


获取列表填充范围。

**Returns:**
java.lang.String
### getListRows() {#getListRows--}
```
public int getListRows()
```


表示列表中要显示的最大行数。

**Returns:**
int
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


获取视觉外观。

参见 [ControlListStyle](../../com.aspose.cells/controlliststyle)。

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


获取宽度（单位为点）。

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


指示 ListBox 或 ComboBox 在用户输入时如何搜索其列表。

参见 [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype)。

**Returns:**
int
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


获取最大字符数

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


获取用于在控件上显示为鼠标指针的自定义图标。

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


获取在控件上显示为鼠标指针的图标类型。

参见 [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype)。

**Returns:**
int
### getSelectionMargin() {#getSelectionMargin--}
```
public boolean getSelectionMargin()
```


指示用户是否可以通过单击文本左侧区域来选择一行文本。

**Returns:**
boolean
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


指示是否显示阴影。

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


指示是否显示列标题。

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


指定下拉按钮上显示的符号

参见 [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype)。

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


获取控件的特殊效果。

参见 [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype)。

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


表示控件使用的文本对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


表示在 ComboBox 或 ListBox 中向用户显示的列。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


获取 ActiveX 控件的类型。

参见 [ControlType](../../com.aspose.cells/controltype)。

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


获取控件的值。

**Returns:**
java.lang.String
### getWidth() {#getWidth--}
```
public double getWidth()
```


获取控件的宽度（单位为点）。

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


获取 [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) 对象。

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


指示控件是否会自动调整大小以显示其全部内容。

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


指定用于扩展选择的基本单位。True 表示基本单位是单个字符。false 表示基本单位是整个单词。

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


指示是否已为控件启用拖放功能。

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


指示用户是否可以在控件中输入。

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


指示控件是否可以获取焦点并响应用户生成的事件。

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


指示控件中的数据是否被锁定，无法编辑。

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


指示控件是否透明。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


指示此控件是否可见。

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


指示控件是否会自动调整大小以显示其全部内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


指定用于扩展选择的基本单位。True 表示基本单位是单个字符。false 表示基本单位是整个单词。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


设置背景的 OLE 颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


设置背景的 OLE 颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


设置控件使用的边框类型。

参见 [ControlBorderType](../../com.aspose.cells/controlbordertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


表示在 MultiSelect 属性值为 (fmMultiSelectSingle) 时，ComboBox 或 ListBox 的 Value 属性的确定方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


表示在 ComboBox 或 ListBox 中显示的列数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


设置列的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


指示是否已为控件启用拖放功能。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


指定下拉按钮上显示的符号

参见 [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


指示用户是否可以在控件中输入。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


指示控件是否可以获取焦点并响应用户生成的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


指定进入控件时的选择行为。True 表示选择保持自上次控件处于活动状态时的状态不变。False 表示进入控件时将选中控件中的所有文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


设置前景的 OLE 颜色。

**Remarks**

不适用于 Image 控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


设置控件的高度（单位为点）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


指示当控件未获得焦点时，控件中的选中文本是否显示为高亮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


设置控件获取焦点时输入法编辑器的默认运行模式。

参见 [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


设置链接的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


设置列表填充范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setListRows(int value) {#setListRows-int-}
```
public void setListRows(int value)
```


表示列表中要显示的最大行数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


设置视觉外观。

参见 [ControlListStyle](../../com.aspose.cells/controlliststyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


设置宽度（单位为点）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


指示控件中的数据是否被锁定，无法编辑。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


指示 ListBox 或 ComboBox 在用户输入时如何搜索其列表。

参见 [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


设置最大字符数

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


设置自定义图标，以在控件上显示为鼠标指针。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


设置在控件上显示为鼠标指针的图标类型。

参见 [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSelectionMargin(boolean value) {#setSelectionMargin-boolean-}
```
public void setSelectionMargin(boolean value)
```


指示用户是否可以通过单击文本左侧区域来选择一行文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


指示是否显示阴影。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


指示是否显示列标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


指定下拉按钮上显示的符号

参见 [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


设置控件的特殊效果。

参见 [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


表示控件使用的文本对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


表示在 ComboBox 或 ListBox 中向用户显示的列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


指示控件是否透明。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


设置控件的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


指示此控件是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


以点为单位设置控件的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

