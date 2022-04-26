---
title: ShapeCollection
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 2620
url: /net/aspose.cells.drawing/shapecollection/
---
## ShapeCollection class

Represents all the shape in a worksheet/chart.

```csharp
public class ShapeCollection : CollectionBase<Shape>
```

## Properties

| Name | Description |
| --- | --- |
| [Item](item) { get; } | Gets the shape object at the specific index. (2 indexers) |

## Methods

| Name | Description |
| --- | --- |
| [AddActiveXControl](addactivexcontrol)(ControlType, int, int, int, int, int, int) | Creates an Activex Control. |
| [AddArc](addarc)(int, int, int, int, int, int) | Adds a ArcShape to the worksheet. |
| [AddAutoShape](addautoshape)(AutoShapeType, int, int, int, int, int, int) | Adds a AutoShape to the worksheet. |
| [AddAutoShapeInChart](addautoshapeinchart)(AutoShapeType, int, int, int, int) | Adds a AutoShape to the chart. |
| [AddButton](addbutton)(int, int, int, int, int, int) | Adds a Button to the worksheet. |
| [AddCheckBox](addcheckbox)(int, int, int, int, int, int) | Adds a checkbox to the worksheet. |
| [AddComboBox](addcombobox)(int, int, int, int, int, int) | Adds a ComboBox to the worksheet. |
| [AddCopy](addcopy)(Shape, int, int, int, int) | Adds and copy a shape to the worksheet. |
| [AddFreeFloatingShape](addfreefloatingshape)(MsoDrawingType, int, int, int, int, byte[], bool) | Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [AddGroupBox](addgroupbox)(int, int, int, int, int, int) | Adds a GroupBox to the worksheet. |
| [AddIcons](addicons)(int, int, int, int, int, int, byte[], byte[]) | Adds svg image. |
| [AddLabel](addlabel)(int, int, int, int, int, int) | Adds a Label to the worksheet. |
| [AddLabelInChart](addlabelinchart)(int, int, int, int) | Adds a label to the chart. |
| [AddLine](addline)(int, int, int, int, int, int) | Adds a LineShape to the worksheet. |
| [AddLinkedPicture](addlinkedpicture)(int, int, int, int, string) | Add a linked picture. |
| [AddListBox](addlistbox)(int, int, int, int, int, int) | Adds a ListBox to the worksheet. |
| [AddOleObject](addoleobject)(int, int, int, int, int, int, byte[]) |  |
| [AddOleObjectWithLinkedImage](addoleobjectwithlinkedimage)(int, int, int, int, string) | Add a linked picture. |
| [AddOval](addoval)(int, int, int, int, int, int) | Adds a Oval to the worksheet. |
| [AddPicture](addpicture)(int, int, int, int, Stream) | Adds a picture to the collection. |
| [AddPicture](addpicture)(int, int, Stream, int, int) | Adds a picture to the collection. |
| [AddPictureInChart](addpictureinchart)(int, int, Stream, int, int) | Adds a picture to the chart. |
| [AddRadioButton](addradiobutton)(int, int, int, int, int, int) | Adds a RadioButton to the worksheet. |
| [AddRectangle](addrectangle)(int, int, int, int, int, int) | Adds a RectangleShape to the worksheet. |
| [AddScrollBar](addscrollbar)(int, int, int, int, int, int) | Adds a ScrollBar to the worksheet. |
| [AddShape](addshape)(MsoDrawingType, int, int, int, int, int, int) | Adds a Shape to the worksheet. |
| [AddShapeInChart](addshapeinchart)(MsoDrawingType, PlacementType, int, int, int, int) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [AddShapeInChart](addshapeinchart)(MsoDrawingType, PlacementType, int, int, int, int, byte[]) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [AddShapeInChartByScale](addshapeinchartbyscale)(MsoDrawingType, PlacementType, double, double, double, double) | Add a shape to chart. All unit is percent scale of chart area. |
| [AddShapeInChartByScale](addshapeinchartbyscale)(MsoDrawingType, PlacementType, double, double, double, double, byte[]) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [AddSpinner](addspinner)(int, int, int, int, int, int) | Adds a Spinner to the worksheet. |
| [AddSvg](addsvg)(int, int, int, int, int, int, byte[], byte[]) | Adds svg image. |
| [AddTextBox](addtextbox)(int, int, int, int, int, int) | Adds a text box to the worksheet. |
| [AddTextBoxInChart](addtextboxinchart)(int, int, int, int) | Adds a textbox to the chart. |
| [AddTextEffect](addtexteffect)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int, int, int) | Inserts a WordArt object. |
| [AddTextEffectInChart](addtexteffectinchart)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int) | Inserts a WordArt object to the chart |
| [AddWordArt](addwordart)(PresetWordArtStyle, string, int, int, int, int, int, int) | Adds preset WordArt since Excel 2007.s |
| [Clear](clear)() | Clear all shapes. |
| [CopyCommentsInRange](copycommentsinrange)(ShapeCollection, CellArea, int, int) | Copy all comments in the range. |
| [CopyInRange](copyinrange)(ShapeCollection, CellArea, int, int, bool) | Copy shapes in the range to destination range. |
| [DeleteInRange](deleteinrange)(CellArea) | Delete shapes in the range.Comment shapes will not be deleted. |
| [DeleteShape](deleteshape)(Shape) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. |
| [Group](group)(Shape[]) | Group the shapes. |
| [Remove](remove)(Shape) | Remove the shape. |
| [RemoveAt](removeat)(int) | Remove the shape. |
| [Ungroup](ungroup)(GroupShape) | Ungroups the shape items. |
| [UpdateSelectedValue](updateselectedvalue)() | Update the selected value by the value of the linked cell of the shapes. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//get ShapeCollection
ShapeCollection shapes = workbook.Worksheets[0].Shapes;

//do your business

//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Shape](../shape)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
