---
title: "Validation 类"
linktitle: "Validation"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Validation 类。封装在 Go 中表示验证的对象。"
type: docs
weight: 200
url: /zh/go-cpp/validation/
---

## Validation class

表示数据验证.settings。

```go

type Validation struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetOperator](./getoperator/) | 表示数据验证的运算符。 |
| [SetOperator](./setoperator/) | 表示数据验证的运算符。 |
| [GetAlertStyle](./getalertstyle/) | 表示验证警报样式。 |
| [SetAlertStyle](./setalertstyle/) | 表示验证警报样式。 |
| [GetType](./gettype/) | 表示数据验证类型。 |
| [SetType](./settype/) | 表示数据验证类型。 |
| [GetInputMessage](./getinputmessage/) | 表示数据验证输入消息。 |
| [SetInputMessage](./setinputmessage/) | 表示数据验证输入消息。 |
| [GetInputTitle](./getinputtitle/) | 表示数据验证输入对话框的标题。 |
| [SetInputTitle](./setinputtitle/) | 表示数据验证输入对话框的标题。 |
| [GetErrorMessage](./geterrormessage/) | 表示数据验证错误消息。 |
| [SetErrorMessage](./seterrormessage/) | 表示数据验证错误消息。 |
| [GetErrorTitle](./geterrortitle/) | 表示数据验证错误对话框的标题。 |
| [SetErrorTitle](./seterrortitle/) | 表示数据验证错误对话框的标题。 |
| [GetShowInput](./getshowinput/) | 指示是否在用户选择数据验证范围内的单元格时显示数据验证输入消息。 |
| [SetShowInput](./setshowinput/) | 指示是否在用户选择数据验证范围内的单元格时显示数据验证输入消息。 |
| [GetShowError](./getshowerror/) | 指示是否在用户输入无效数据时显示数据验证错误消息。 |
| [SetShowError](./setshowerror/) | 指示是否在用户输入无效数据时显示数据验证错误消息。 |
| [GetIgnoreBlank](./getignoreblank/) | 指示范围数据验证是否允许空白值。 |
| [SetIgnoreBlank](./setignoreblank/) | 指示范围数据验证是否允许空白值。 |
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | 获取与此验证关联的值或表达式。 |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | 获取与此验证关联的值或表达式。 |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | 获取与特定单元格的此验证关联的值或表达式。 |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | 获取与特定单元格的此验证关联的值或表达式。 |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | 设置与此验证关联的值或表达式。 |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | 设置与此验证关联的值或表达式。 |
| [GetFormula1](./getformula1/) | 表示与数据验证关联的值或表达式。 |
| [SetFormula1_String](./setformula1_string/) | 表示与数据验证关联的值或表达式。 |
| [GetFormula2](./getformula2/) | 表示与数据验证关联的值或表达式。 |
| [SetFormula2_String](./setformula2_string/) | 表示与数据验证关联的值或表达式。 |
| [GetListValue](./getlistvalue/) | 获取指定单元格的验证列表的值。 |
| [GetValue1](./getvalue1/) | 表示与数据验证关联的第一个值。 |
| [SetValue1](./setvalue1/) | 表示与数据验证关联的第一个值。 |
| [GetValue2](./getvalue2/) | 表示与数据验证关联的第二个值。 |
| [SetValue2](./setvalue2/) | 表示与数据验证关联的第二个值。 |
| [GetValue](./getvalue/) | 获取特定单元格上验证的值。 |
| [GetInCellDropDown](./getincelldropdown/) | 指示数据验证是否显示包含可接受值的下拉列表。 |
| [SetInCellDropDown](./setincelldropdown/) | 指示数据验证是否显示包含可接受值的下拉列表。 |
| [GetAreas](./getareas/) | 获取包含数据验证设置的所有 CellArea。 |
| [AddArea_CellArea](./addarea_cellarea/) | 将验证应用于该区域。 |
| [AddArea_CellArea_Bool_Bool](./addarea_cellarea_bool_bool/) | 将验证应用于该区域。 |
| [AddAreas](./addareas/) | 将验证应用于给定的区域。 |
| [RemoveArea](./removearea/) | 删除范围内的验证设置。 |
| [RemoveAreas](./removeareas/) | 从给定的区域中移除此验证。 |
| [RemoveACell](./removeacell/) | 删除单元格中的验证设置。 |
| [Copy](./copy/) | 复制验证。 |
