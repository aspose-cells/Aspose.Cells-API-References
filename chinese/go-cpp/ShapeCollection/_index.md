---
title: "ShapeCollection 类"
linktitle: "ShapeCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ShapeCollection 类。封装在 Go 中表示 shapecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/shapecollection/
---

## ShapeCollection class

表示工作表/图表中的所有形状。

```go

type ShapeCollection struct  {
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
| [Get_Int](./get_int/) | 获取列表中特定索引处的 Shape 对象。 |
| [Get_String](./get_string/) | 通过形状名称获取 Shape 对象。 |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | 向工作表添加并复制形状。 |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | 向工作表添加并复制形状。 |
| [AddCheckBox](./addcheckbox/) | 向工作表添加复选框。 |
| [AddTextBox](./addtextbox/) | 向工作表添加文本框。 |
| [AddEquation](./addequation/) | 向工作表添加公式对象。 |
| [AddLaTeXEquation](./addlatexequation/) | 使用 LaTeX 格式字符串向工作表添加公式对象。 |
| [AddSpinner](./addspinner/) | 向工作表添加微调器。 |
| [AddScrollBar](./addscrollbar/) | 向工作表添加滚动条。 |
| [AddRadioButton](./addradiobutton/) | 向工作表添加单选按钮。 |
| [AddListBox](./addlistbox/) | 向工作表添加列表框。 |
| [AddComboBox](./addcombobox/) | 向工作表添加下拉框。 |
| [AddGroupBox](./addgroupbox/) | 向工作表添加组框。 |
| [AddButton](./addbutton/) | 向工作表添加按钮。 |
| [AddLabel](./addlabel/) | 向工作表添加标签。 |
| [AddLabelInChart](./addlabelinchart/) | 向图表添加标签。 |
| [AddTextBoxInChart](./addtextboxinchart/) | 向图表添加文本框。 |
| [AddTextEffectInChart](./addtexteffectinchart/) | 向图表插入 WordArt 对象 |
| [AddTextEffect](./addtexteffect/) | 插入 WordArt 对象。 |
| [AddWordArt](./addwordart/) | 添加自 Excel 2007 起的预设 WordArt。 |
| [AddRectangle](./addrectangle/) | 向工作表添加矩形形状。 |
| [AddOval](./addoval/) | 向工作表添加椭圆。 |
| [AddLine](./addline/) | 向工作表添加线形状。 |
| [AddFreeFloatingShape](./addfreefloatingshape/) | 向工作表添加自由浮动形状。仅适用于线形或图像形状。 |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | 向图表添加形状。所有单位为图表区域的百分比比例。 |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [AddArc](./addarc/) | 向工作表添加弧形。 |
| [AddShape](./addshape/) | 向工作表添加形状。 |
| [AddAutoShape](./addautoshape/) | 向工作表添加自动形状。 |
| [AddAutoShapeInChart](./addautoshapeinchart/) | 向图表添加自动形状。 |
| [AddActiveXControl](./addactivexcontrol/) | 创建 ActiveX 控件。 |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | 向集合中添加图片。 |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | 向集合中添加图片。 |
| [AddSvg](./addsvg/) | 添加 svg 图像。 |
| [AddIcons](./addicons/) | 添加 svg 图像。 |
| [AddLinkedPicture](./addlinkedpicture/) | 添加一个链接图片。 |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | 添加一个链接图片。 |
| [AddPictureInChart](./addpictureinchart/) | 向图表添加图片。 |
| [AddOleObject](./addoleobject/) | 添加 OleObject。 |
| [CopyCommentsInRange](./copycommentsinrange/) | 复制范围内的所有批注。 |
| [CopyInRange](./copyinrange/) | 将范围内的形状复制到目标范围。 |
| [DeleteInRange](./deleteinrange/) | 删除范围内的形状。注释形状将不会被删除。 |
| [DeleteShape](./deleteshape/) | 删除形状。如果该形状位于组中或是注释形状，则不会被删除。 |
| [Group](./group/) | 对形状进行分组。 |
| [Ungroup](./ungroup/) | 取消形状项目的分组。 |
| [RemoveAt](./removeat/) | 移除形状。 |
| [Remove](./remove/) | 移除形状。 |
| [Clear](./clear/) | 清除工作表中的所有形状。 |
| [UpdateSelectedValue](./updateselectedvalue/) | 通过链接单元格或形状范围的值更新所选值。 |
| [AddFreeform](./addfreeform/) | 向工作表添加自由形状。 |
| [AddSignatureLine](./addsignatureline/) | 向工作表添加签名行。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
