---
title: ShapeCollection Class 
linktitle: ShapeCollection
second_title: Aspose.Cells for Go via C++ API Reference
description: 'ShapeCollection class. Encapsulates the object that represents shapecollection in Go.'
type: docs
weight: 200
url: /go-cpp/shapecollection/
---

## ShapeCollection class

Represents all the shape in a worksheet/chart.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Get_Int](./get_int/) | Gets the Shape object at the specific index in the list. | 
|[Get_String](./get_string/) | Gets the Shape object by the name of the shape. | 
|[AddCopy](./addcopy/) | Adds and copy a shape to the worksheet. | 
|[AddCheckBox](./addcheckbox/) | Adds a checkbox to the worksheet. | 
|[AddTextBox](./addtextbox/) | Adds a text box to the worksheet. | 
|[AddEquation](./addequation/) | Adds an equation object to the worksheet. | 
|[AddLaTeXEquation](./addlatexequation/) | Adds an equation object to the worksheet using LaTeX format strings. | 
|[AddSpinner](./addspinner/) | Adds a Spinner to the worksheet. | 
|[AddScrollBar](./addscrollbar/) | Adds a ScrollBar to the worksheet. | 
|[AddRadioButton](./addradiobutton/) | Adds a RadioButton to the worksheet. | 
|[AddListBox](./addlistbox/) | Adds a ListBox to the worksheet. | 
|[AddComboBox](./addcombobox/) | Adds a ComboBox to the worksheet. | 
|[AddGroupBox](./addgroupbox/) | Adds a GroupBox to the worksheet. | 
|[AddButton](./addbutton/) | Adds a Button to the worksheet. | 
|[AddLabel](./addlabel/) | Adds a Label to the worksheet. | 
|[AddLabelInChart](./addlabelinchart/) | Adds a label to the chart. | 
|[AddTextBoxInChart](./addtextboxinchart/) | Adds a textbox to the chart. | 
|[AddTextEffectInChart](./addtexteffectinchart/) | Inserts a WordArt object to the chart | 
|[AddTextEffect](./addtexteffect/) | Inserts a WordArt object. | 
|[AddWordArt](./addwordart/) | Adds preset WordArt since Excel 2007.s | 
|[AddRectangle](./addrectangle/) | Adds a RectangleShape to the worksheet. | 
|[AddOval](./addoval/) | Adds a Oval to the worksheet. | 
|[AddLine](./addline/) | Adds a LineShape to the worksheet. | 
|[AddFreeFloatingShape](./addfreefloatingshape/) | Adds a free floating shape to the worksheet.Only applies for line/image shape. | 
|[AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Add a shape to chart .All unit is 1/4000 of chart area. | 
|[AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Add a shape to chart .All unit is 1/4000 of chart area. | 
|[AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Add a shape to chart. All unit is percent scale of chart area. | 
|[AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Add a shape to chart .All unit is 1/4000 of chart area. | 
|[AddArc](./addarc/) | Adds a ArcShape to the worksheet. | 
|[AddShape](./addshape/) | Adds a Shape to the worksheet. | 
|[AddAutoShape](./addautoshape/) | Adds a AutoShape to the worksheet. | 
|[AddAutoShapeInChart](./addautoshapeinchart/) | Adds a AutoShape to the chart. | 
|[AddActiveXControl](./addactivexcontrol/) | Creates an Activex Control. | 
|[AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Adds a picture to the collection. | 
|[AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Adds a picture to the collection. | 
|[AddSvg](./addsvg/) | Adds svg image. | 
|[AddIcons](./addicons/) | Adds svg image. | 
|[AddLinkedPicture](./addlinkedpicture/) | Add a linked picture. | 
|[AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Add a linked picture. | 
|[AddPictureInChart](./addpictureinchart/) | Adds a picture to the chart. | 
|[AddOleObject](./addoleobject/) | Adds an OleObject. | 
|[CopyCommentsInRange](./copycommentsinrange/) | Copy all comments in the range. | 
|[CopyInRange](./copyinrange/) | Copy shapes in the range to destination range. | 
|[DeleteInRange](./deleteinrange/) | Delete shapes in the range.Comment shapes will not be deleted. | 
|[DeleteShape](./deleteshape/) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. | 
|[Group](./group/) | Group the shapes. | 
|[Ungroup](./ungroup/) | Ungroups the shape items. | 
|[RemoveAt](./removeat/) | Remove the shape. | 
|[Remove](./remove/) | Remove the shape. | 
|[Clear](./clear/) | Clear all shapes in the worksheet. | 
|[UpdateSelectedValue](./updateselectedvalue/) | Update the selected value by the value of the linked cell or range of the shape. | 
|[AddFreeform](./addfreeform/) | Adds a freeform shape to the worksheet. | 
|[AddSignatureLine](./addsignatureline/) | Adds a Signature Line to the worksheet. | 
|[GetCount](./getcount/) |  | 
