---
title: "TextBoxActiveXControl 类"
linktitle: "TextBoxActiveXControl"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TextBoxActiveXControl 类。封装在 Go 中表示 textboxactivexcontrol 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/textboxactivexcontrol/
---

## TextBoxActiveXControl class

表示文本框 ActiveX 控件。

```go

type TextBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewTextBoxActiveXControl](./newtextboxactivexcontrol/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetType](./gettype/) | 获取 ActiveX 控件的类型。 |
| [GetBorderStyle](./getborderstyle/) | 获取并设置控件使用的边框类型。 |
| [SetBorderStyle](./setborderstyle/) | 获取并设置控件使用的边框类型。 |
| [GetBorderOleColor](./getborderolecolor/) | 获取并设置背景的 OLE 颜色。 |
| [SetBorderOleColor](./setborderolecolor/) | 获取并设置背景的 OLE 颜色。 |
| [GetSpecialEffect](./getspecialeffect/) | 获取并设置控件的特殊效果。 |
| [SetSpecialEffect](./setspecialeffect/) | 获取并设置控件的特殊效果。 |
| [GetMaxLength](./getmaxlength/) | 获取并设置最大字符数 |
| [SetMaxLength](./setmaxlength/) | 获取并设置最大字符数 |
| [GetScrollBars](./getscrollbars/) | 指示控件是否具有垂直滚动条、水平滚动条、两者皆有或两者皆无。 |
| [SetScrollBars](./setscrollbars/) | 指示控件是否具有垂直滚动条、水平滚动条、两者皆有或两者皆无。 |
| [GetPasswordChar](./getpasswordchar/) | 获取和设置用于替代已输入字符的显示字符。 |
| [SetPasswordChar](./setpasswordchar/) | 获取和设置用于替代已输入字符的显示字符。 |
| [IsEditable](./iseditable/) | 指示用户是否可以在控件中输入。 |
| [SetIsEditable](./setiseditable/) | 指示用户是否可以在控件中输入。 |
| [GetIntegralHeight](./getintegralheight/) | 指示该控件是否仅显示完整的文本行，而不显示任何部分行。 |
| [SetIntegralHeight](./setintegralheight/) | 指示该控件是否仅显示完整的文本行，而不显示任何部分行。 |
| [IsDragBehaviorEnabled](./isdragbehaviorenabled/) | 指示是否为控件启用拖放功能。 |
| [SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | 指示是否为控件启用拖放功能。 |
| [GetEnterKeyBehavior](./getenterkeybehavior/) | 指定 ENTER 键的行为。True 表示按下 ENTER 将创建新行。False 表示按下 ENTER 将把焦点移动到选项卡顺序中的下一个对象。 |
| [SetEnterKeyBehavior](./setenterkeybehavior/) | 指定 ENTER 键的行为。True 表示按下 ENTER 将创建新行。False 表示按下 ENTER 将把焦点移动到选项卡顺序中的下一个对象。 |
| [GetEnterFieldBehavior](./getenterfieldbehavior/) | 指定进入控件时的选择行为。True 表示选择保持自上次控件激活时不变。False 表示进入控件时将选择控件中的全部文本。 |
| [SetEnterFieldBehavior](./setenterfieldbehavior/) | 指定进入控件时的选择行为。True 表示选择保持自上次控件激活时不变。False 表示进入控件时将选择控件中的全部文本。 |
| [GetTabKeyBehavior](./gettabkeybehavior/) | 指示是否允许在控件的文本中使用制表符。 |
| [SetTabKeyBehavior](./settabkeybehavior/) | 指示是否允许在控件的文本中使用制表符。 |
| [GetHideSelection](./gethideselection/) | 指示当控件失去焦点时，已选择的文本是否显示为高亮。 |
| [SetHideSelection](./sethideselection/) | 指示当控件失去焦点时，已选择的文本是否显示为高亮。 |
| [IsAutoTab](./isautotab/) | 指示当用户输入的字符数达到最大值时，焦点是否会自动移动到下一个控件。 |
| [SetIsAutoTab](./setisautotab/) | 指示当用户输入的字符数达到最大值时，焦点是否会自动移动到下一个控件。 |
| [IsMultiLine](./ismultiline/) | 指示控件是否可以显示多行文本。 |
| [SetIsMultiLine](./setismultiline/) | 指示控件是否可以显示多行文本。 |
| [IsWordWrapped](./iswordwrapped/) | 指示控件的内容是否在行尾自动换行。 |
| [SetIsWordWrapped](./setiswordwrapped/) | 指示控件的内容是否在行尾自动换行。 |
| [GetText](./gettext/) | 获取和设置控件的文本。 |
| [SetText](./settext/) | 获取和设置控件的文本。 |
| [GetDropButtonStyle](./getdropbuttonstyle/) | 指定下拉按钮上显示的符号 |
| [SetDropButtonStyle](./setdropbuttonstyle/) | 指定下拉按钮上显示的符号 |
| [GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | 指定下拉按钮上显示的符号 |
| [SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | 指定下拉按钮上显示的符号 |
| [IsAutoWordSelected](./isautowordselected/) | 指定用于扩展选择的基本单位。True 表示基本单位为单个字符。false 表示基本单位为整个单词。 |
| [SetIsAutoWordSelected](./setisautowordselected/) | 指定用于扩展选择的基本单位。True 表示基本单位为单个字符。false 表示基本单位为整个单词。 |
| [IsEnabled](./isenabled/) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [SetIsEnabled](./setisenabled/) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [IsLocked](./islocked/) | 指示控件中的数据是否被锁定以进行编辑。 |
| [SetIsLocked](./setislocked/) | 指示控件中的数据是否被锁定以进行编辑。 |
| [IsTransparent](./istransparent/) | 指示控件是否透明。 |
| [SetIsTransparent](./setistransparent/) | 指示控件是否透明。 |
| [GetIMEMode](./getimemode/) | 获取和设置控件在获得焦点时输入法编辑器的默认运行时模式。 |
| [SetIMEMode](./setimemode/) | 获取和设置控件在获得焦点时输入法编辑器的默认运行时模式。 |
| [GetFont](./getfont/) | 表示控件的字体。 |
| [GetTextAlign](./gettextalign/) | 表示控件使用的文本的对齐方式。 |
| [SetTextAlign](./settextalign/) | 表示控件使用的文本的对齐方式。 |
| [GetData](./getdata/) | 获取并设置控件的二进制数据。 |
| [IsAutoSize](./isautosize/) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [SetIsAutoSize](./setisautosize/) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [GetWorkbook](./getworkbook/) | 获取 Workbook 对象。 |
| [GetMouseIcon](./getmouseicon/) | 获取并设置用于在控件上显示为鼠标指针的自定义图标。 |
| [SetMouseIcon](./setmouseicon/) | 获取并设置用于在控件上显示为鼠标指针的自定义图标。 |
| [GetMousePointer](./getmousepointer/) | 获取并设置在控件上显示为鼠标指针的图标类型。 |
| [SetMousePointer](./setmousepointer/) | 获取并设置在控件上显示为鼠标指针的图标类型。 |
| [GetLinkedCell](./getlinkedcell/) | 获取并设置链接的单元格。 |
| [SetLinkedCell](./setlinkedcell/) | 获取并设置链接的单元格。 |
| [GetListFillRange](./getlistfillrange/) | 获取并设置列表填充范围。 |
| [SetListFillRange](./setlistfillrange/) | 获取并设置列表填充范围。 |
| [GetWidth](./getwidth/) | 获取并设置控件的宽度（单位为点）。 |
| [SetWidth](./setwidth/) | 获取并设置控件的宽度（单位为点）。 |
| [GetHeight](./getheight/) | 获取并设置控件的高度（单位为点）。 |
| [SetHeight](./setheight/) | 获取并设置控件的高度（单位为点）。 |
| [GetForeOleColor](./getforeolecolor/) | 获取并设置前景的 OLE 颜色。 |
| [SetForeOleColor](./setforeolecolor/) | 获取并设置前景的 OLE 颜色。 |
| [GetBackOleColor](./getbackolecolor/) | 获取并设置背景的 OLE 颜色。 |
| [SetBackOleColor](./setbackolecolor/) | 获取并设置背景的 OLE 颜色。 |
| [IsVisible](./isvisible/) | 指示此控件是否可见。 |
| [SetIsVisible](./setisvisible/) | 指示此控件是否可见。 |
| [GetShadow](./getshadow/) | 指示是否显示阴影。 |
| [SetShadow](./setshadow/) | 指示是否显示阴影。 |
