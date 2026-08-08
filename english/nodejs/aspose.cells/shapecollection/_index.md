---
title: "ShapeCollection"
linktitle: "ShapeCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents all the shape in a worksheet/chart."
type: docs
weight: 3560
url: /nodejs/aspose.cells/shapecollection/
---

## ShapeCollection class

Represents all the shape in a worksheet/chart.

## Methods

| Name | Description |
| --- | --- |
| [addActiveXControl(type, topRow, top, leftColumn, left, height, width)](./addactivexcontrol/) | Creates an Activex Control. |
| [addArc(upperLeftRow, top, upperLeftColumn, left, height, width)](./addarc/) | Adds a ArcShape to the worksheet. |
| [addAutoShape(type, upperLeftRow, top, upperLeftColumn, left, height, width)](./addautoshape/) | Adds a AutoShape to the worksheet. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addAutoShapeInChart(type, top, left, height, width)](./addautoshapeinchart/) | Adds a AutoShape to the chart. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addButton(upperLeftRow, top, upperLeftColumn, left, height, width)](./addbutton/) | Adds a Button to the worksheet. |
| [addCheckBox(upperLeftRow, top, upperLeftColumn, left, height, width)](./addcheckbox/) | Adds a checkbox to the worksheet. |
| [addComboBox(upperLeftRow, top, upperLeftColumn, left, height, width)](./addcombobox/) | Adds a ComboBox to the worksheet. |
| [addCopy(sourceShape, topRow, top, leftColumn, left)](./addcopy/) | Adds and copy a shape to the worksheet. |
| [addCopy()](./addcopy-1/) |  |
| [addEquation(topRow, top, leftColumn, left, height, width)](./addequation/) | Add an equation object to the worksheet. |
| [addFreeFloatingShape(type, top, left, height, width, imageData, isOriginalSize)](./addfreefloatingshape/) | Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [addFreeform()](./addfreeform/) |  |
| [addGroupBox(upperLeftRow, top, upperLeftColumn, left, height, width)](./addgroupbox/) | Adds a GroupBox to the worksheet. |
| [addIcons(upperLeftRow, top, upperLeftColumn, left, height, width, imageByteData, compatibleImageData)](./addicons/) | Adds svg image. |
| [addLaTeXEquation()](./addlatexequation/) |  |
| [addLabel(upperLeftRow, top, upperLeftColumn, left, height, width)](./addlabel/) | Adds a Label to the worksheet. |
| [addLabelInChart(top, left, height, width)](./addlabelinchart/) | Adds a label to the chart. |
| [addLine(upperLeftRow, top, upperLeftColumn, left, height, width)](./addline/) | Adds a LineShape to the worksheet. |
| [addLinkedPicture(upperLeftRow, upperLeftColumn, height, width, sourceFullName)](./addlinkedpicture/) | Add a linked picture. |
| [addListBox(upperLeftRow, top, upperLeftColumn, left, height, width)](./addlistbox/) | Adds a ListBox to the worksheet. |
| [addOleObject(upperLeftRow, top, upperLeftColumn, left, height, width, imageData)](./addoleobject/) | Adds an OleObject. |
| [addOleObjectWithLinkedImage(upperLeftRow, upperLeftColumn, height, width, sourceFullName)](./addoleobjectwithlinkedimage/) | Add a linked picture. |
| [addOval(upperLeftRow, top, upperLeftColumn, left, height, width)](./addoval/) | Adds a Oval to the worksheet. |
| [addRadioButton(upperLeftRow, top, upperLeftColumn, left, height, width)](./addradiobutton/) | Adds a RadioButton to the worksheet. |
| [addRectangle(upperLeftRow, top, upperLeftColumn, left, height, width)](./addrectangle/) | Adds a RectangleShape to the worksheet. |
| [addScrollBar(upperLeftRow, top, upperLeftColumn, left, height, width)](./addscrollbar/) | Adds a ScrollBar to the worksheet. |
| [addShape(type, upperLeftRow, top, upperLeftColumn, left, height, width)](./addshape/) | Adds a Shape to the worksheet. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addShapeInChart(type, placement, left, top, right, bottom, imageData)](./addshapeinchart/) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChart(type, placement, left, top, right, bottom)](./addshapeinchart-1/) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChartByScale(type, placement, left, top, right, bottom)](./addshapeinchartbyscale/) | Add a shape to chart. All unit is percent scale of chart area. |
| [addShapeInChartByScale(type, placement, left, top, right, bottom, imageData)](./addshapeinchartbyscale-1/) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addSignatureLine()](./addsignatureline/) |  |
| [addSpinner(upperLeftRow, top, upperLeftColumn, left, height, width)](./addspinner/) | Adds a Spinner to the worksheet. |
| [addSvg(upperLeftRow, top, upperLeftColumn, left, height, width, svgData, compatibleImageData)](./addsvg/) | Adds svg image. |
| [addTextBox(upperLeftRow, top, upperLeftColumn, left, height, width)](./addtextbox/) | Adds a text box to the worksheet. |
| [addTextBoxInChart(top, left, height, width)](./addtextboxinchart/) | Adds a textbox to the chart. |
| [addTextEffect(effect, text, fontName, size, fontBold, fontItalic, upperLeftRow, top, upperLeftColumn, left, height, width)](./addtexteffect/) | Inserts a WordArt object. |
| [addTextEffectInChart(effect, text, fontName, size, fontBold, fontItalic, top, left, height, width)](./addtexteffectinchart/) | Inserts a WordArt object to the chart |
| [addWordArt(style, text, upperLeftRow, top, upperLeftColumn, left, height, width)](./addwordart/) | Adds preset WordArt since Excel 2007.s |
| [clear()](./clear/) | Clear all shapes in the worksheet. |
| [contains()](./contains/) | Reserved for internal use. |
| [copyCommentsInRange(shapes, ca, destRow, destColumn)](./copycommentsinrange/) | Copy all comments in the range. |
| [copyInRange(sourceShapes, ca, destRow, destColumn, isContained)](./copyinrange/) | Copy shapes in the range to destination range. |
| [deleteInRange(ca)](./deleteinrange/) | Delete shapes in the range.Comment shapes will not be deleted. |
| [deleteShape(shape)](./deleteshape/) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. |
| [get(index)](./get/) | Gets the Shape object at the specific index in the list. |
| [get(name)](./get-1/) | Gets the Shape object by the name of the shape. |
| [get()](./get-2/) | Reserved for internal use. |
| [getCount()](./getcount/) |  |
| [group(groupItems)](./group/) | Group the shapes. The shape in the groupItems should not be grouped. The shape must be in this Shapes collection. |
| [indexOf()](./indexof/) | Reserved for internal use. |
| [iterator()](./iterator/) |  |
| [remove(shape)](./remove/) | Remove the shape. |
| [removeAt(index)](./removeat/) | Remove the shape. |
| [ungroup(group)](./ungroup/) | Ungroups the shape items. If the group shape is grouped by another group shape,nothing will be done. |
| [updateSelectedValue()](./updateselectedvalue/) | Update the selected value by the value of the linked cell or range of the shape. |
| [addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, stream, callback)](./addpicturefromstream/) *(static)* | Adds a picture to the collection. |
| [addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, widthScale, heightScale, callback)](./addpicturefromstream-1/) *(static)* | Adds a picture to the collection. |
| [addPictureInChartFromStream(pictures, top, left, stream, widthScale, heightScale, callback)](./addpictureinchartfromstream/) *(static)* | Adds a picture to the chart. |
