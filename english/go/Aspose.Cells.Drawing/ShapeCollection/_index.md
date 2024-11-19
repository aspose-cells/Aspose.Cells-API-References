---
title: ShapeCollection Class 
linktitle: ShapeCollection
second_title: Aspose.Cells for Go API Reference
description: 'ShapeCollection class. Encapsulates the object that represents shapecollection in Go.'
type: docs
weight: 200
url: /go/aspose.cells.drawing/shapecollection/
---

## ShapeCollection class

Represents all the shape in a worksheet/chart.

```go

type ShapeCollection struct 

shapecollection, _ := asposecells.NewShapeCollection()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewShapeCollection](./newshapecollection/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Get](./get/) | Gets the <see cref="Shape"/> object at the specific index in the list. | 
|[Get](./get/) | Gets the <see cref="Shape"/> object by the name of the shape. | 
|[AddCopy](./addcopy/) | Adds and copy a shape to the worksheet. | 
|[AddCheckBox](./addcheckbox/) | Adds a checkbox to the worksheet. | 
|[AddTextBox](./addtextbox/) | Adds a text box to the worksheet. | 
|[AddEquation](./addequation/) | Add an equation object to the worksheet. | 
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
|[AddShapeInChart](./addshapeinchart/) | Add a shape to chart .All unit is 1/4000 of chart area. | 
|[AddShapeInChartByScale](./addshapeinchartbyscale/) | Add a shape to chart. All unit is percent scale of chart area. | 
|[AddArc](./addarc/) | Adds a ArcShape to the worksheet. | 
|[AddShape](./addshape/) | Adds a Shape to the worksheet. | 
|[AddAutoShape](./addautoshape/) | Adds a AutoShape to the worksheet. | 
|[AddAutoShapeInChart](./addautoshapeinchart/) | Adds a AutoShape to the chart. | 
|[AddActiveXControl](./addactivexcontrol/) | Creates an Activex Control. | 
|[AddLinkedPicture](./addlinkedpicture/) | Add a linked picture. | 
|[AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Add a linked picture. | 
|[CopyCommentsInRange](./copycommentsinrange/) | Copy all comments in the range. | 
|[CopyInRange](./copyinrange/) | Copy shapes in the range to destination range. | 
|[DeleteInRange](./deleteinrange/) | Delete shapes in the range.Comment shapes will not be deleted. | 
|[DeleteShape](./deleteshape/) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. | 
|[Ungroup](./ungroup/) | Ungroups the shape items. | 
|[RemoveAt](./removeat/) | Remove the shape. | 
|[Remove](./remove/) | Remove the shape. | 
|[Clear](./clear/) | Clear all shapes in the worksheet. | 
|[UpdateSelectedValue](./updateselectedvalue/) | Update the selected value by the value of the linked cell or range of the shape. | 
|[AddSignatureLine](./addsignatureline/) | Adds a Signature Line to the worksheet. | 
|[GetCount](./getcount/) |  | 
