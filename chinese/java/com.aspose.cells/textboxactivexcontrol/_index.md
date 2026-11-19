---
title: "TextBoxActiveXControl"
second_title: "Aspose.Cells for Java API 参考"
description: "表示文本框 ActiveX 控件。"
type: docs
url: /zh/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

表示文本框 ActiveX 控件。

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a TextBoxActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50);
         TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | 获取背景的 ole 颜色。 |
| [getBorderOleColor()](#getBorderOleColor--) | 获取背景的 ole 颜色。 |
| [getBorderStyle()](#getBorderStyle--) | 获取控件使用的边框类型。 |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | 获取控件的二进制数据。 |
| [getDropButtonStyle()](#getDropButtonStyle--) | 指定下拉按钮上显示的符号 |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | 指定进入控件时的选择行为。 |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | 指定 ENTER 键的行为。 |
| [getFont()](#getFont--) | 表示控件的字体。 |
| [getForeOleColor()](#getForeOleColor--) | 获取前景的 OLE 颜色。 |
| [getHeight()](#getHeight--) | 获取控件的高度（单位为点）。 |
| [getHideSelection()](#getHideSelection--) | 指示当控件未获得焦点时，控件中的选中文本是否显示为高亮。 |
| [getIMEMode()](#getIMEMode--) | 获取控件获得焦点时输入法编辑器的默认运行模式。 |
| [getIntegralHeight()](#getIntegralHeight--) | 指示控件是否仅显示完整的文本行，而不显示任何部分行。 |
| [getLinkedCell()](#getLinkedCell--) | 获取链接的单元格。 |
| [getListFillRange()](#getListFillRange--) | 获取列表填充范围。 |
| [getMaxLength()](#getMaxLength--) | 获取最大字符数 |
| [getMouseIcon()](#getMouseIcon--) | 获取用于在控件上显示为鼠标指针的自定义图标。 |
| [getMousePointer()](#getMousePointer--) | 获取在控件上显示为鼠标指针的图标类型。 |
| [getPasswordChar()](#getPasswordChar--) | 获取用于替代已输入字符显示的字符。 |
| [getScrollBars()](#getScrollBars--) | 指示指定控件是否具有垂直滚动条、水平滚动条、两者兼有或两者皆无。 |
| [getShadow()](#getShadow--) | 指示是否显示阴影。 |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | 指定下拉按钮上显示的符号 |
| [getSpecialEffect()](#getSpecialEffect--) | 获取控件的特殊效果。 |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | 指示控件的文本中是否允许制表符。 |
| [getText()](#getText--) | 获取控件的文本。 |
| [getTextAlign()](#getTextAlign--) | 表示控件使用的文本对齐方式。 |
| [getType()](#getType--) | 获取 ActiveX 控件的类型。 |
| [getWidth()](#getWidth--) | 获取控件的宽度（单位为点）。 |
| [getWorkbook()](#getWorkbook--) | 获取 [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) 对象。 |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [isAutoTab()](#isAutoTab--) | 指示当用户输入的字符数达到最大值时，焦点是否会自动移动到下一个控件。 |
| [isAutoWordSelected()](#isAutoWordSelected--) | 指定用于扩展选择的基本单位。 |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | 指示是否已为控件启用拖放功能。 |
| [isEditable()](#isEditable--) | 指示用户是否可以在控件中输入。 |
| [isEnabled()](#isEnabled--) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [isLocked()](#isLocked--) | 指示控件中的数据是否被锁定，无法编辑。 |
| [isMultiLine()](#isMultiLine--) | 指示控件是否可以显示多行文本。 |
| [isTransparent()](#isTransparent--) | 指示控件是否透明。 |
| [isVisible()](#isVisible--) | 指示此控件是否可见。 |
| [isWordWrapped()](#isWordWrapped--) | 指示控件的内容是否在行尾自动换行。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | 指示当用户输入的字符数达到最大值时，焦点是否会自动移动到下一个控件。 |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | 指定用于扩展选择的基本单位。 |
| [setBackOleColor(int value)](#setBackOleColor-int-) | 设置背景的 OLE 颜色。 |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | 设置背景的 OLE 颜色。 |
| [setBorderStyle(int value)](#setBorderStyle-int-) | 设置控件使用的边框类型。 |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | 指示是否已为控件启用拖放功能。 |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | 指定下拉按钮上显示的符号 |
| [setEditable(boolean value)](#setEditable-boolean-) | 指示用户是否可以在控件中输入。 |
| [setEnabled(boolean value)](#setEnabled-boolean-) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | 指定进入控件时的选择行为。 |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | 指定 ENTER 键的行为。 |
| [setForeOleColor(int value)](#setForeOleColor-int-) | 设置前景的 OLE 颜色。 |
| [setHeight(double value)](#setHeight-double-) | 设置控件的高度（单位为点）。 |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | 指示当控件未获得焦点时，控件中的选中文本是否显示为高亮。 |
| [setIMEMode(int value)](#setIMEMode-int-) | 设置控件获取焦点时输入法编辑器的默认运行模式。 |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | 指示控件是否仅显示完整的文本行，而不显示任何部分行。 |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | 设置链接的单元格。 |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | 设置列表填充范围。 |
| [setLocked(boolean value)](#setLocked-boolean-) | 指示控件中的数据是否被锁定，无法编辑。 |
| [setMaxLength(int value)](#setMaxLength-int-) | 设置最大字符数 |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | 设置自定义图标，以在控件上显示为鼠标指针。 |
| [setMousePointer(int value)](#setMousePointer-int-) | 设置在控件上显示为鼠标指针的图标类型。 |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | 指示控件是否可以显示多行文本。 |
| [setPasswordChar(char value)](#setPasswordChar-char-) | 设置一个字符，以在输入的字符位置显示该字符。 |
| [setScrollBars(int value)](#setScrollBars-int-) | 指示指定控件是否具有垂直滚动条、水平滚动条、两者兼有或两者皆无。 |
| [setShadow(boolean value)](#setShadow-boolean-) | 指示是否显示阴影。 |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | 指定下拉按钮上显示的符号 |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | 设置控件的特殊效果。 |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | 指示控件的文本中是否允许制表符。 |
| [setText(String value)](#setText-java.lang.String-) | 设置控件的文本。 |
| [setTextAlign(int value)](#setTextAlign-int-) | 表示控件使用的文本对齐方式。 |
| [setTransparent(boolean value)](#setTransparent-boolean-) | 指示控件是否透明。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示此控件是否可见。 |
| [setWidth(double value)](#setWidth-double-) | 以点为单位设置控件的宽度。 |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | 指示控件的内容是否在行尾自动换行。 |
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

**Example**

```
         //excel default color system 12 or green(0x0000FF00)
         activeXControl.setBorderOleColor(/*unchecked*/((int)0x80000012L));
```

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


获取控件使用的边框类型。

参见 [ControlBorderType](../../com.aspose.cells/controlbordertype)。

**Example**

```
         activeXControl.setBorderStyle(com.aspose.cells.ControlBorderType.SINGLE);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

**Example**

```
         activeXControl.setDropButtonStyle(com.aspose.cells.DropButtonStyle.ARROW);
```

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


指定进入控件时的选择行为。True 表示选择保持自上次控件处于活动状态时的状态不变。False 表示进入控件时将选中控件中的所有文本。

**Example**

```
         if(!activeXControl.getEnterFieldBehavior())
         {
             activeXControl.setEnterFieldBehavior(true);
         }
```

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


指定 ENTER 键的行为。True 表示按下 ENTER 将创建新行。False 表示按下 ENTER 将把焦点移动到选项卡顺序中的下一个对象。

**Example**

```
         if(!activeXControl.getEnterKeyBehavior())
         {
             activeXControl.setEnterKeyBehavior(true);
         }
```

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

**Example**

```
         if(!activeXControl.getHideSelection())
         {
             activeXControl.setHideSelection(true);
         }
```

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
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


指示控件是否仅显示完整的文本行，而不显示任何部分行。

**Example**

```
         if(!activeXControl.getIntegralHeight())
         {
             activeXControl.setIntegralHeight(true);
         }
```

**Returns:**
boolean
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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


获取最大字符数

**Example**

```
         if(activeXControl.getMaxLength() == 0)
         {
             activeXControl.setMaxLength(30);
         }
```

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
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


获取用于替代已输入字符显示的字符。

**Example**

```
         activeXControl.setPasswordChar('a');
```

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


指示指定控件是否具有垂直滚动条、水平滚动条、两者兼有或两者皆无。

参见 [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype)。

**Example**

```
         activeXControl.setScrollBars(com.aspose.cells.ControlScrollBarType.BARS_VERTICAL);
```

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


指示是否显示阴影。

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


指定下拉按钮上显示的符号

参见 [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype)。

**Example**

```
         activeXControl.setShowDropButtonTypeWhen(com.aspose.cells.ShowDropButtonType.FOCUS);
```

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


获取控件的特殊效果。

参见 [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype)。

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
```

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


指示控件的文本中是否允许制表符。

**Example**

```
         if(!activeXControl.getTabKeyBehavior())
         {
             activeXControl.setTabKeyBehavior(true);
         }
```

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


获取控件的文本。

**Example**

```
         activeXControl.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


表示控件使用的文本对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


获取 ActiveX 控件的类型。

参见 [ControlType](../../com.aspose.cells/controltype)。

**Example**

```
         /*Aspose.Cells.Drawing.ActiveXControls.ControlType*/int type = activeXControl.getType();
```

**Returns:**
int
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
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


指示当用户输入的字符数达到最大值时，焦点是否会自动移动到下一个控件。

**Example**

```
         if(!activeXControl.isAutoTab())
         {
             activeXControl.setAutoTab(true);
         }
```

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


指定用于扩展选择的基本单位。True 表示基本单位是单个字符。false 表示基本单位是整个单词。

**Example**

```
         if(!activeXControl.isAutoWordSelected())
         {
             activeXControl.setAutoWordSelected(true);
         }
```

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


指示是否已为控件启用拖放功能。

**Example**

```
         if(!activeXControl.isDragBehaviorEnabled())
         {
             activeXControl.setDragBehaviorEnabled(true);
         }
```

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


指示用户是否可以在控件中输入。

**Example**

```
         if(!activeXControl.isEditable())
         {
             activeXControl.setEditable(true);
         }
```

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
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


指示控件是否可以显示多行文本。

**Example**

```
         if(!activeXControl.isMultiLine())
         {
             activeXControl.setMultiLine(true);
         }
```

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
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


指示控件的内容是否在行尾自动换行。

**Example**

```
         if(!activeXControl.isWordWrapped())
         {
             activeXControl.setWordWrapped(true);
         }
```

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

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


指示当用户输入的字符数达到最大值时，焦点是否会自动移动到下一个控件。

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

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


指定 ENTER 键的行为。True 表示按下 ENTER 将创建新行。False 表示按下 ENTER 将把焦点移动到选项卡顺序中的下一个对象。

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

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


指示控件是否仅显示完整的文本行，而不显示任何部分行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


指示控件中的数据是否被锁定，无法编辑。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


指示控件是否可以显示多行文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


设置一个字符，以在输入的字符位置显示该字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


指示指定控件是否具有垂直滚动条、水平滚动条、两者兼有或两者皆无。

参见 [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


指示是否显示阴影。

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

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


指示控件的文本中是否允许制表符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


设置控件的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


指示控件是否透明。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


指示控件的内容是否在行尾自动换行。

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

