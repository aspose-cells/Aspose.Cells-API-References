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
| [addActiveXControl(type, topRow, top, leftColumn, left, height, width)](#addactivexcontrol) | Creates an Activex Control. |
| [addArc(upperLeftRow, top, upperLeftColumn, left, height, width)](#addarc) | Adds a ArcShape to the worksheet. |
| [addAutoShape(type, upperLeftRow, top, upperLeftColumn, left, height, width)](#addautoshape) | Adds a AutoShape to the worksheet. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addAutoShapeInChart(type, top, left, height, width)](#addautoshapeinchart) | Adds a AutoShape to the chart. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addButton(upperLeftRow, top, upperLeftColumn, left, height, width)](#addbutton) | Adds a Button to the worksheet. |
| [addCheckBox(upperLeftRow, top, upperLeftColumn, left, height, width)](#addcheckbox) | Adds a checkbox to the worksheet. |
| [addComboBox(upperLeftRow, top, upperLeftColumn, left, height, width)](#addcombobox) | Adds a ComboBox to the worksheet. |
| [addCopy(sourceShape, topRow, top, leftColumn, left)](#addcopy) | Adds and copy a shape to the worksheet. |
| [addCopy()](#addcopy-1) |  |
| [addEquation(topRow, top, leftColumn, left, height, width)](#addequation) | Add an equation object to the worksheet. |
| [addFreeFloatingShape(type, top, left, height, width, imageData, isOriginalSize)](#addfreefloatingshape) | Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [addFreeform()](#addfreeform) |  |
| [addGroupBox(upperLeftRow, top, upperLeftColumn, left, height, width)](#addgroupbox) | Adds a GroupBox to the worksheet. |
| [addIcons(upperLeftRow, top, upperLeftColumn, left, height, width, imageByteData, compatibleImageData)](#addicons) | Adds svg image. |
| [addLaTeXEquation()](#addlatexequation) |  |
| [addLabel(upperLeftRow, top, upperLeftColumn, left, height, width)](#addlabel) | Adds a Label to the worksheet. |
| [addLabelInChart(top, left, height, width)](#addlabelinchart) | Adds a label to the chart. |
| [addLine(upperLeftRow, top, upperLeftColumn, left, height, width)](#addline) | Adds a LineShape to the worksheet. |
| [addLinkedPicture(upperLeftRow, upperLeftColumn, height, width, sourceFullName)](#addlinkedpicture) | Add a linked picture. |
| [addListBox(upperLeftRow, top, upperLeftColumn, left, height, width)](#addlistbox) | Adds a ListBox to the worksheet. |
| [addOleObject(upperLeftRow, top, upperLeftColumn, left, height, width, imageData)](#addoleobject) | Adds an OleObject. |
| [addOleObjectWithLinkedImage(upperLeftRow, upperLeftColumn, height, width, sourceFullName)](#addoleobjectwithlinkedimage) | Add a linked picture. |
| [addOval(upperLeftRow, top, upperLeftColumn, left, height, width)](#addoval) | Adds a Oval to the worksheet. |
| [addRadioButton(upperLeftRow, top, upperLeftColumn, left, height, width)](#addradiobutton) | Adds a RadioButton to the worksheet. |
| [addRectangle(upperLeftRow, top, upperLeftColumn, left, height, width)](#addrectangle) | Adds a RectangleShape to the worksheet. |
| [addScrollBar(upperLeftRow, top, upperLeftColumn, left, height, width)](#addscrollbar) | Adds a ScrollBar to the worksheet. |
| [addShape(type, upperLeftRow, top, upperLeftColumn, left, height, width)](#addshape) | Adds a Shape to the worksheet. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addShapeInChart(type, placement, left, top, right, bottom, imageData)](#addshapeinchart) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChart(type, placement, left, top, right, bottom)](#addshapeinchart-1) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChartByScale(type, placement, left, top, right, bottom)](#addshapeinchartbyscale) | Add a shape to chart. All unit is percent scale of chart area. |
| [addShapeInChartByScale(type, placement, left, top, right, bottom, imageData)](#addshapeinchartbyscale-1) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addSignatureLine()](#addsignatureline) |  |
| [addSpinner(upperLeftRow, top, upperLeftColumn, left, height, width)](#addspinner) | Adds a Spinner to the worksheet. |
| [addSvg(upperLeftRow, top, upperLeftColumn, left, height, width, svgData, compatibleImageData)](#addsvg) | Adds svg image. |
| [addTextBox(upperLeftRow, top, upperLeftColumn, left, height, width)](#addtextbox) | Adds a text box to the worksheet. |
| [addTextBoxInChart(top, left, height, width)](#addtextboxinchart) | Adds a textbox to the chart. |
| [addTextEffect(effect, text, fontName, size, fontBold, fontItalic, upperLeftRow, top, upperLeftColumn, left, height, width)](#addtexteffect) | Inserts a WordArt object. |
| [addTextEffectInChart(effect, text, fontName, size, fontBold, fontItalic, top, left, height, width)](#addtexteffectinchart) | Inserts a WordArt object to the chart |
| [addWordArt(style, text, upperLeftRow, top, upperLeftColumn, left, height, width)](#addwordart) | Adds preset WordArt since Excel 2007.s |
| [clear()](#clear) | Clear all shapes in the worksheet. |
| [contains()](#contains) | Reserved for internal use. |
| [copyCommentsInRange(shapes, ca, destRow, destColumn)](#copycommentsinrange) | Copy all comments in the range. |
| [copyInRange(sourceShapes, ca, destRow, destColumn, isContained)](#copyinrange) | Copy shapes in the range to destination range. |
| [deleteInRange(ca)](#deleteinrange) | Delete shapes in the range.Comment shapes will not be deleted. |
| [deleteShape(shape)](#deleteshape) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. |
| [get(index)](#get) | Gets the Shape object at the specific index in the list. |
| [get(name)](#get-1) | Gets the Shape object by the name of the shape. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [group(groupItems)](#group) | Group the shapes. The shape in the groupItems should not be grouped. The shape must be in this Shapes collection. |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(shape)](#remove) | Remove the shape. |
| [removeAt(index)](#removeat) | Remove the shape. |
| [ungroup(group)](#ungroup) | Ungroups the shape items. If the group shape is grouped by another group shape,nothing will be done. |
| [updateSelectedValue()](#updateselectedvalue) | Update the selected value by the value of the linked cell or range of the shape. |
| [addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, stream, callback)](#addpicturefromstream) *(static)* | Adds a picture to the collection. |
| [addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, widthScale, heightScale, callback)](#addpicturefromstream-1) *(static)* | Adds a picture to the collection. |
| [addPictureInChartFromStream(pictures, top, left, stream, widthScale, heightScale, callback)](#addpictureinchartfromstream) *(static)* | Adds a picture to the chart. |

### addActiveXControl(type, topRow, top, leftColumn, left, height, width) {#addactivexcontrol}

Creates an Activex Control.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ControlType |
| topRow | Number | Upper left row index. |
| top | Number | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | Number | Upper left column index. |
| left | Number | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Number | Represents the height of Shape, in unit of pixel. |
| width | Number | Represents the width of Shape, in unit of pixel. |

**Returns:** Shape — `Shape`

### addArc(upperLeftRow, top, upperLeftColumn, left, height, width) {#addarc}

Adds a ArcShape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of ArcShape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of ArcShape from its left column, in unit of pixel. |
| height | Number | Represents the height of ArcShape, in unit of pixel. |
| width | Number | Represents the width of ArcShape, in unit of pixel. |

**Returns:** ArcShape — `ArcShape` A ArcShape object.

### addAutoShape(type, upperLeftRow, top, upperLeftColumn, left, height, width) {#addautoshape}

Adds a AutoShape to the worksheet. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | AutoShapeType |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Number | Represents the height of Shape, in unit of pixel. |
| width | Number | Represents the width of Shape, in unit of pixel. |

**Returns:** Shape — `Shape` A Shape object.

### addAutoShapeInChart(type, top, left, height, width) {#addautoshapeinchart}

Adds a AutoShape to the chart. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | AutoShapeType |
| top | Number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | Number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | Number | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | Number | Represents the width of textbox, in units of 1/4000 of the chart area. |

**Returns:** Shape — `Shape` Returns a shape object.

### addButton(upperLeftRow, top, upperLeftColumn, left, height, width) {#addbutton}

Adds a Button to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of Button from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of Button from its left column, in unit of pixel. |
| height | Number | Represents the height of Button, in unit of pixel. |
| width | Number | Represents the width of Button, in unit of pixel. |

**Returns:** Button — `Button` A Button object.

### addCheckBox(upperLeftRow, top, upperLeftColumn, left, height, width) {#addcheckbox}

Adds a checkbox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of checkbox from its top row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | Number | Height of textbox, in unit of pixel. |
| width | Number | Width of textbox, in unit of pixel. |

**Returns:** CheckBox — `CheckBox` The new CheckBox object index.

### addComboBox(upperLeftRow, top, upperLeftColumn, left, height, width) {#addcombobox}

Adds a ComboBox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of ComboBox from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of ComboBox from its left column, in unit of pixel. |
| height | Number | Represents the height of ComboBox, in unit of pixel. |
| width | Number | Represents the width of ComboBox, in unit of pixel. |

**Returns:** ComboBox — `ComboBox` A ComboBox object.

### addCopy(sourceShape, topRow, top, leftColumn, left) {#addcopy}

Adds and copy a shape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | Shape | Source shape. |
| topRow | Number | The top row index. |
| top | Number | Represents the vertical offset from its top row, in unit of pixel. |
| leftColumn | Number | The left column index. |
| left | Number | Represents the horizontal offset from its left column, in unit of pixel. |

**Returns:** Shape — `Shape` The new Shape object.

### addCopy() {#addcopy-1}

### addEquation(topRow, top, leftColumn, left, height, width) {#addequation}

Add an equation object to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Number | The top row index. |
| top | Number | The vertical offset its top row, in unit of pixel. |
| leftColumn | Number | The left column index. |
| left | Number | The horizontal offset from its left column, in unit of pixel. |
| height | Number | The height of equation, in unit of pixel. |
| width | Number | The width of equation, in unit of pixel. |

**Returns:** TextBox — `TextBox`

### addFreeFloatingShape(type, top, left, height, width, imageData, isOriginalSize) {#addfreefloatingshape}

Adds a free floating shape to the worksheet.Only applies for line/image shape.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | MsoDrawingType |
| top | Number | Represents the vertical offset of shape from the worksheet's top row, in unit of pixel. |
| left | Number | Represents the horizontal offset of shape from the worksheet's left column, in unit of pixel. |
| height | Number | Represents the height of LineShape, in unit of pixel. |
| width | Number | Represents the width of LineShape, in unit of pixel. |
| imageData | Array of byte | The image data,only applies for the picture. |
| isOriginalSize | boolean | Whether the shape use original size if the shape is image. |

**Returns:** Shape — `Shape`

### addFreeform() {#addfreeform}

### addGroupBox(upperLeftRow, top, upperLeftColumn, left, height, width) {#addgroupbox}

Adds a GroupBox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of GroupBox from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of GroupBox from its left column, in unit of pixel. |
| height | Number | Represents the height of GroupBox, in unit of pixel. |
| width | Number | Represents the width of GroupBox, in unit of pixel. |

**Returns:** GroupBox — `GroupBox` A GroupBox object.

### addIcons(upperLeftRow, top, upperLeftColumn, left, height, width, imageByteData, compatibleImageData) {#addicons}

Adds svg image.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | The horizontal offset of shape from its left column, in unit of pixel. |
| height | Number | The height of shape, in unit of pixel. |
| width | Number | The width of shape, in unit of pixel. |
| imageByteData | Array of byte | The image byte data. |
| compatibleImageData | Array of byte | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

**Returns:** Picture — `Picture`

### addLaTeXEquation() {#addlatexequation}

### addLabel(upperLeftRow, top, upperLeftColumn, left, height, width) {#addlabel}

Adds a Label to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of Label from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of Label from its left column, in unit of pixel. |
| height | Number | Represents the height of Label, in unit of pixel. |
| width | Number | Represents the width of Label, in unit of pixel. |

**Returns:** Label — `Label` A Label object.

### addLabelInChart(top, left, height, width) {#addlabelinchart}

Adds a label to the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| top | Number | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| left | Number | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| height | Number | Represents the height of label, in units of 1/4000 of the chart area. |
| width | Number | Represents the width of label, in units of 1/4000 of the chart area. |

**Returns:** Label — `Label` A new Label object.

### addLine(upperLeftRow, top, upperLeftColumn, left, height, width) {#addline}

Adds a LineShape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of LineShape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of LineShape from its left column, in unit of pixel. |
| height | Number | Represents the height of LineShape, in unit of pixel. |
| width | Number | Represents the width of LineShape, in unit of pixel. |

**Returns:** LineShape — `LineShape` A LineShape object.

### addLinkedPicture(upperLeftRow, upperLeftColumn, height, width, sourceFullName) {#addlinkedpicture}

Add a linked picture.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | Number | The height of the shape. In unit of pixels |
| width | Number | The width of the shape. In unit of pixels |
| sourceFullName | String | The path and name of the source file for the linked image |

**Returns:** Picture — `Picture` Picture Picture object.

### addListBox(upperLeftRow, top, upperLeftColumn, left, height, width) {#addlistbox}

Adds a ListBox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of ListBox from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of ListBox from its left column, in unit of pixel. |
| height | Number | Represents the height of ListBox, in unit of pixel. |
| width | Number | Represents the width of ListBox, in unit of pixel. |

**Returns:** ListBox — `ListBox` A ListBox object.

### addOleObject(upperLeftRow, top, upperLeftColumn, left, height, width, imageData) {#addoleobject}

Adds an OleObject.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  |  |
| top | Number |  |
| upperLeftColumn |  |  |
| left | Number |  |
| height | Number |  |
| width | Number |  |
| imageData | Array of byte |  |

**Returns:** OleObject — `OleObject`

### addOleObjectWithLinkedImage(upperLeftRow, upperLeftColumn, height, width, sourceFullName) {#addoleobjectwithlinkedimage}

Add a linked picture.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | Number | The height of the shape. In unit of pixels |
| width | Number | The width of the shape. In unit of pixels |
| sourceFullName | String | The path and name of the source file for the linked image |

**Returns:** OleObject — `OleObject` Picture Picture object.

### addOval(upperLeftRow, top, upperLeftColumn, left, height, width) {#addoval}

Adds a Oval to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of Oval from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of Oval from its left column, in unit of pixel. |
| height | Number | Represents the height of Oval, in unit of pixel. |
| width | Number | Represents the width of Oval, in unit of pixel. |

**Returns:** Oval — `Oval` A Oval object.

### addRadioButton(upperLeftRow, top, upperLeftColumn, left, height, width) {#addradiobutton}

Adds a RadioButton to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of RadioButton from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of RadioButton from its left column, in unit of pixel. |
| height | Number | Represents the height of RadioButton, in unit of pixel. |
| width | Number | Represents the width of RadioButton, in unit of pixel. |

**Returns:** RadioButton — `RadioButton` A RadioButton object.

### addRectangle(upperLeftRow, top, upperLeftColumn, left, height, width) {#addrectangle}

Adds a RectangleShape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of RectangleShape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of RectangleShape from its left column, in unit of pixel. |
| height | Number | Represents the height of RectangleShape, in unit of pixel. |
| width | Number | Represents the width of RectangleShape, in unit of pixel. |

**Returns:** RectangleShape — `RectangleShape` A RectangleShape object.

### addScrollBar(upperLeftRow, top, upperLeftColumn, left, height, width) {#addscrollbar}

Adds a ScrollBar to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of ScrollBar from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of ScrollBar from its left column, in unit of pixel. |
| height | Number | Represents the height of ScrollBar, in unit of pixel. |
| width | Number | Represents the width of ScrollBar, in unit of pixel. |

**Returns:** ScrollBar — `ScrollBar` A ScrollBar object.

### addShape(type, upperLeftRow, top, upperLeftColumn, left, height, width) {#addshape}

Adds a Shape to the worksheet. The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | MsoDrawingType |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Number | Represents the height of Shape, in unit of pixel. |
| width | Number | Represents the width of Shape, in unit of pixel. |

**Returns:** Shape — `Shape` A Shape object.

### addShapeInChart(type, placement, left, top, right, bottom, imageData) {#addshapeinchart}

Add a shape to chart .All unit is 1/4000 of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | MsoDrawingType |
| placement | Number | PlacementType |
| left | Number | In unit of 1/4000 chart area width. |
| top | Number | In unit of 1/4000 chart area height. |
| right | Number | In unit of 1/4000 chart area width. |
| bottom | Number | In unit of 1/4000 chart area height. |
| imageData | Array of byte | If the shape is not a picture or ole object,imageData should be null. |

### addShapeInChart(type, placement, left, top, right, bottom) {#addshapeinchart-1}

Add a shape to chart .All unit is 1/4000 of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | MsoDrawingType |
| placement | Number | PlacementType |
| left | Number | In unit of 1/4000 chart area width. |
| top | Number | In unit of 1/4000 chart area height. |
| right | Number | In unit of 1/4000 chart area width. |
| bottom | Number | In unit of 1/4000 chart area height. |

### addShapeInChartByScale(type, placement, left, top, right, bottom) {#addshapeinchartbyscale}

Add a shape to chart. All unit is percent scale of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | MsoDrawingType |
| placement | Number | PlacementType |
| left | Number | Unit is percent scale of chart area width. |
| top | Number | Unit is percent scale of chart area height. |
| right | Number | Unit is percent scale of chart area width. |
| bottom | Number | Unit is percent scale of chart area height. |

### addShapeInChartByScale(type, placement, left, top, right, bottom, imageData) {#addshapeinchartbyscale-1}

Add a shape to chart .All unit is 1/4000 of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | MsoDrawingType |
| placement | Number | PlacementType |
| left | Number | Unit is percent scale of chart area width. |
| top | Number | Unit is percent scale of chart area height. |
| right | Number | Unit is percent scale of chart area width. |
| bottom | Number | Unit is percent scale of chart area height. |
| imageData | Array of byte | If the shape is not a picture or ole object,imageData should be null. |

### addSignatureLine() {#addsignatureline}

### addSpinner(upperLeftRow, top, upperLeftColumn, left, height, width) {#addspinner}

Adds a Spinner to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of Spinner from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of Spinner from its left column, in unit of pixel. |
| height | Number | Represents the height of Spinner, in unit of pixel. |
| width | Number | Represents the width of Spinner, in unit of pixel. |

**Returns:** Spinner — `Spinner` A Spinner object.

### addSvg(upperLeftRow, top, upperLeftColumn, left, height, width, svgData, compatibleImageData) {#addsvg}

Adds svg image.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | The horizontal offset of shape from its left column, in unit of pixel. |
| height | Number | The height of shape, in unit of pixel. |
| width | Number | The width of shape, in unit of pixel. |
| svgData | Array of byte | The svg image data. |
| compatibleImageData | Array of byte | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

**Returns:** Picture — `Picture`

### addTextBox(upperLeftRow, top, upperLeftColumn, left, height, width) {#addtextbox}

Adds a text box to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of textbox from its top row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | Number | Represents the height of textbox, in unit of pixel. |
| width | Number | Represents the width of textbox, in unit of pixel. |

**Returns:** TextBox — `TextBox` A TextBox object.

### addTextBoxInChart(top, left, height, width) {#addtextboxinchart}

Adds a textbox to the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| top | Number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | Number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | Number | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | Number | Represents the width of textbox, in units of 1/4000 of the chart area. |

**Returns:** TextBox — `TextBox` A TextBox object.

### addTextEffect(effect, text, fontName, size, fontBold, fontItalic, upperLeftRow, top, upperLeftColumn, left, height, width) {#addtexteffect}

Inserts a WordArt object.

| Parameter | Type | Description |
| --- | --- | --- |
| effect | Number | MsoPresetTextEffect |
| text | String | The WordArt text. |
| fontName | String | The font name. |
| size | Number | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | Number | Represents the height of shape, in unit of pixel. |
| width | Number | Represents the width of shape, in unit of pixel. |

**Returns:** Shape — `Shape` Returns a Shape object that represents the new WordArt object.

### addTextEffectInChart(effect, text, fontName, size, fontBold, fontItalic, top, left, height, width) {#addtexteffectinchart}

Inserts a WordArt object to the chart

| Parameter | Type | Description |
| --- | --- | --- |
| effect | Number | MsoPresetTextEffect |
| text | String | The WordArt text. |
| fontName | String | The font name. |
| size | Number | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| top | Number | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | Number | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| height | Number | Represents the height of shape, in units of 1/4000 of the chart area. |
| width | Number | Represents the width of shape, in units of 1/4000 of the chart area. |

**Returns:** Shape — `Shape` Returns a Shape object that represents the new WordArt object.

### addWordArt(style, text, upperLeftRow, top, upperLeftColumn, left, height, width) {#addwordart}

Adds preset WordArt since Excel 2007.s

| Parameter | Type | Description |
| --- | --- | --- |
| style | Number | PresetWordArtStyle |
| text | String | The text. |
| upperLeftRow |  | Upper left row index. |
| top | Number | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | Number | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | Number | Represents the height of shape, in unit of pixel. |
| width | Number | Represents the width of shape, in unit of pixel. |

**Returns:** Shape — `Shape`

### clear() {#clear}

Clear all shapes in the worksheet.

### contains() {#contains}

Reserved for internal use.

### copyCommentsInRange(shapes, ca, destRow, destColumn) {#copycommentsinrange}

Copy all comments in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| shapes | ShapeCollection | The source shapes. |
| ca | CellArea | The source range. |
| destRow | Number | The dest range start row. |
| destColumn | Number | The dest range start column. |

### copyInRange(sourceShapes, ca, destRow, destColumn, isContained) {#copyinrange}

Copy shapes in the range to destination range.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Source shapes. |
| ca | CellArea | The source range. |
| destRow | Number | The dest row index of the dest range. |
| destColumn | Number | The dest column of the dest range. |
| isContained | boolean | Whether only copy the shapes which are contained in the range. If true,only copies the shapes in the range. Otherwise,it works as MS Office. |

### deleteInRange(ca) {#deleteinrange}

Delete shapes in the range.Comment shapes will not be deleted.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range.If the shapes are contained in the range, they will be removed. |

### deleteShape(shape) {#deleteshape}

Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.

| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape |  |

### get(index) {#get}

Gets the Shape object at the specific index in the list.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index. |

**Returns:** Shape — `Shape`

### get(name) {#get-1}

Gets the Shape object by the name of the shape.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the shape. |

**Returns:** Shape — `Shape`

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### group(groupItems) {#group}

Group the shapes. The shape in the groupItems should not be grouped. The shape must be in this Shapes collection.

| Parameter | Type | Description |
| --- | --- | --- |
| groupItems | Array ofShape | the group items. |

**Returns:** GroupShape — `GroupShape` Return the group shape.

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### remove(shape) {#remove}

Remove the shape.

| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape |  |

### removeAt(index) {#removeat}

Remove the shape.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the shape. |

### ungroup(group) {#ungroup}

Ungroups the shape items. If the group shape is grouped by another group shape,nothing will be done.

| Parameter | Type | Description |
| --- | --- | --- |
| group | GroupShape | The group shape. |

### updateSelectedValue() {#updateselectedvalue}

Update the selected value by the value of the linked cell or range of the shape.

### addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, stream, callback) (static) {#addpicturefromstream}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| pictures | PictureCollection | The PictureCollection object |
| upperLeftRow | Number | Upper left row index |
| upperLeftColumn | Number | Upper left column index |
| lowerRightRow | Number | Lower right row index |
| lowerRightColumn | Number | Lower right column index |
| stream | ReadableStream | Stream object which contains the image data |
| callback | Callback | The callback function |

**Returns:** object — `object` Returns a Picture objct

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var shapes = workbook.getWorksheets().get(0).getShapes();
var shapeStream = fs.createReadStream("boxing.PNG");
aspose.cells.ShapeCollection.addPictureFromStream(shapes, 1, 1, 10, 5, shapeStream,
function(picture, err) {
if (!err) {
console.log("addPictureFromStream done");
}
workbook.save('result.xlsx');
}
);
```

### addPictureFromStream(pictures, upperLeftRow, upperLeftColumn, stream, widthScale, heightScale, callback) (static) {#addpicturefromstream-1}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| pictures | PictureCollection | The PictureCollection object |
| upperLeftRow | Number | Upper left row index |
| upperLeftColumn | Number | Upper left column index |
| stream | ReadableStream | Stream object which contains the image data |
| widthScale | Number | Scale of image width, a percentage |
| heightScale | Number | Scale of image height, a percentage |
| callback | Callback | The callback function |

**Returns:** object — `object` Returns a Picture objct

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook();
var shapes = workbook.getWorksheets().get(0).getShapes();
var shapeStream = fs.createReadStream("boxing.PNG");
aspose.cells.ShapeCollection.addPictureFromStream(shapes, 1, 1, shapeStream, 80, 60,
function(picture, err) {
if (!err) {
console.log("addPictureFromStream done");
}
workbook.save('result.xlsx');
}
);
```

### addPictureInChartFromStream(pictures, top, left, stream, widthScale, heightScale, callback) (static) {#addpictureinchartfromstream}

Adds a picture to the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| pictures | PictureCollection | The PictureCollection object |
| top | Number | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area |
| left | Number | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area |
| stream | ReadableStream | Stream object which contains the image data |
| widthScale | Number | Scale of image width, a percentage |
| heightScale | Number | Scale of image height, a percentage |
| callback | Callback | The callback function |

**Returns:** object — `object` Returns a Picture objct

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var shapes = workbook.getWorksheets().get("Chart").getCharts().get(0).getShapes();
var shapeStream = fs.createReadStream("boxing.PNG");
aspose.cells.ShapeCollection.addPictureInChartFromStream(shapes, 1, 1, shapeStream, 10, 5,
function(picture, err) {
if (!err) {
console.log("addPictureInChartFromStream done");
}
workbook.save('result.xlsx');
}
);
```
