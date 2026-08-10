---
title: "ShapeCollection Class"
linktitle: "ShapeCollection"
articleTitle: "ShapeCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents all the shape in a worksheet/chart."
type: docs
weight: 5820
url: /python-java/asposecells.api/shapecollection/
---

## ShapeCollection class

Represents all the shape in a worksheet/chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | Shape | Gets the Shape object at the specific index in the list. |
| [Item (java.lang.String)](#itemjavalangstring) | Shape | Gets the Shape object by the name of the shape. |

## Methods

| Name | Description |
| --- | --- |
| [addCopy](#addcopy) | Adds and copy a shape to the worksheet. |
| [addCheckBox](#addcheckbox) | Adds a checkbox to the worksheet. |
| [addTextBox](#addtextbox) | Adds a text box to the worksheet. |
| [addEquation](#addequation) | Add an equation object to the worksheet. |
| [addLaTeXEquation](#addlatexequation) |  |
| [addSpinner](#addspinner) | Adds a Spinner to the worksheet. |
| [addScrollBar](#addscrollbar) | Adds a ScrollBar to the worksheet. |
| [addRadioButton](#addradiobutton) | Adds a RadioButton to the worksheet. |
| [addListBox](#addlistbox) | Adds a ListBox to the worksheet. |
| [addComboBox](#addcombobox) | Adds a ComboBox to the worksheet. |
| [addGroupBox](#addgroupbox) | Adds a GroupBox to the worksheet. |
| [addButton](#addbutton) | Adds a Button to the worksheet. |
| [addLabel](#addlabel) | Adds a Label to the worksheet. |
| [addLabelInChart](#addlabelinchart) | Adds a label to the chart. |
| [addTextBoxInChart](#addtextboxinchart) | Adds a textbox to the chart. |
| [addTextEffectInChart](#addtexteffectinchart) | Inserts a WordArt object to the chart |
| [addTextEffect](#addtexteffect) | Inserts a WordArt object. |
| [addWordArt](#addwordart) | Adds preset WordArt since Excel 2007.s |
| [addRectangle](#addrectangle) | Adds a RectangleShape to the worksheet. |
| [addOval](#addoval) | Adds a Oval to the worksheet. |
| [addLine](#addline) | Adds a LineShape to the worksheet. |
| [addFreeFloatingShape](#addfreefloatingshape) | Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [addShapeInChart](#addshapeinchart) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChartByScale](#addshapeinchartbyscale) | Add a shape to chart. All unit is percent scale of chart area. |
| [addArc](#addarc) | Adds a ArcShape to the worksheet. |
| [addShape](#addshape) | Adds a Shape to the worksheet.

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addAutoShape](#addautoshape) | Adds a AutoShape to the worksheet.

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addAutoShapeInChart](#addautoshapeinchart) | Adds a AutoShape to the chart.

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox |
| [addActiveXControl](#addactivexcontrol) | Creates an Activex Control. |
| [addSvg](#addsvg) | Adds svg image. |
| [addIcons](#addicons) | Adds svg image. |
| [addLinkedPicture](#addlinkedpicture) | Add a linked picture. |
| [addOleObjectWithLinkedImage](#addoleobjectwithlinkedimage) | Add a linked picture. |
| [addOleObject](#addoleobject) | Adds an OleObject. |
| [copyCommentsInRange](#copycommentsinrange) | Copy all comments in the range. |
| [copyInRange](#copyinrange) | Copy shapes in the range to destination range. |
| [deleteInRange](#deleteinrange) | Delete shapes in the range.Comment shapes will not be deleted. |
| [deleteShape](#deleteshape) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. |
| [group](#group) | Group the shapes.

The shape in the groupItems should not be grouped. The shape must be in this Shapes collection. |
| [ungroup](#ungroup) | Ungroups the shape items.

If the group shape is grouped by another group shape,nothing will be done. |
| [removeAt](#removeat) | Remove the shape. |
| [remove](#remove) | Remove the shape. |
| [clear](#clear) | Clear all shapes in the worksheet. |
| [updateSelectedValue](#updateselectedvalue) | Update the selected value by the value of the linked cell or range of the shape. |
| [addFreeform](#addfreeform) |  |
| [addSignatureLine](#addsignatureline) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |
| [addPictureFromBytes](#addpicturefrombytes) | Adds a picture to the collection. |
| [addPictureInChartFromBytes](#addpictureinchartfrombytes) | Adds a picture to the chart. |

### ShapeCollection.Count property {#count}

**Type:** int

### ShapeCollection.Item (int) property {#itemint}

Gets the Shape object at the specific index in the list.

**Type:** Shape

### ShapeCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the Shape object by the name of the shape.

**Type:** Shape

### addCopy(sourceShape, topRow, top, leftColumn, left) (1 of 2) {#addcopy}

Adds and copy a shape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | Shape | Source shape. |
| topRow | int | The top row index. |
| top | int | Represents the vertical offset from its top row, in unit of pixel. |
| leftColumn | int | The left column index. |
| left | int | Represents the horizontal offset from its left column, in unit of pixel. |

**Returns:** The new Shape object.

---

### addCopy(sourceShape, topRow, top, leftColumn, left, copyOptions) (2 of 2) {#addcopy-1}

### addCheckBox(topRow, top, leftColumn, left, height, width) {#addcheckbox}

Adds a checkbox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of checkbox from its top row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int | Height of textbox, in unit of pixel. |
| width | int | Width of textbox, in unit of pixel. |

**Returns:** The new CheckBox object index.

### addTextBox(topRow, top, leftColumn, left, height, width) {#addtextbox}

Adds a text box to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of textbox from its top row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int | Represents the height of textbox, in unit of pixel. |
| width | int | Represents the width of textbox, in unit of pixel. |

**Returns:** A TextBox object.

### addEquation(topRow, top, leftColumn, left, height, width) {#addequation}

Add an equation object to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | The top row index. |
| top | int | The vertical offset its top row, in unit of pixel. |
| leftColumn | int | The left column index. |
| left | int | The horizontal offset from its left column, in unit of pixel. |
| height | int | The height of equation, in unit of pixel. |
| width | int | The width of equation, in unit of pixel. |

### addLaTeXEquation(topRow, top, leftColumn, left, height, width, latex) {#addlatexequation}

### addSpinner(topRow, top, leftColumn, left, height, width) {#addspinner}

Adds a Spinner to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of Spinner from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of Spinner from its left column, in unit of pixel. |
| height | int | Represents the height of Spinner, in unit of pixel. |
| width | int | Represents the width of Spinner, in unit of pixel. |

**Returns:** A Spinner object.

### addScrollBar(topRow, top, leftColumn, left, height, width) {#addscrollbar}

Adds a ScrollBar to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of ScrollBar from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of ScrollBar from its left column, in unit of pixel. |
| height | int | Represents the height of ScrollBar, in unit of pixel. |
| width | int | Represents the width of ScrollBar, in unit of pixel. |

**Returns:** A ScrollBar object.

### addRadioButton(topRow, top, leftColumn, left, height, width) {#addradiobutton}

Adds a RadioButton to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of RadioButton from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of RadioButton from its left column, in unit of pixel. |
| height | int | Represents the height of RadioButton, in unit of pixel. |
| width | int | Represents the width of RadioButton, in unit of pixel. |

**Returns:** A RadioButton object.

### addListBox(topRow, top, leftColumn, left, height, width) {#addlistbox}

Adds a ListBox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of ListBox from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of ListBox from its left column, in unit of pixel. |
| height | int | Represents the height of ListBox, in unit of pixel. |
| width | int | Represents the width of ListBox, in unit of pixel. |

**Returns:** A ListBox object.

### addComboBox(topRow, top, leftColumn, left, height, width) {#addcombobox}

Adds a ComboBox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of ComboBox from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of ComboBox from its left column, in unit of pixel. |
| height | int | Represents the height of ComboBox, in unit of pixel. |
| width | int | Represents the width of ComboBox, in unit of pixel. |

**Returns:** A ComboBox object.

### addGroupBox(topRow, top, leftColumn, left, height, width) {#addgroupbox}

Adds a GroupBox to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of GroupBox from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of GroupBox from its left column, in unit of pixel. |
| height | int | Represents the height of GroupBox, in unit of pixel. |
| width | int | Represents the width of GroupBox, in unit of pixel. |

**Returns:** A GroupBox object.

### addButton(topRow, top, leftColumn, left, height, width) {#addbutton}

Adds a Button to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of Button from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of Button from its left column, in unit of pixel. |
| height | int | Represents the height of Button, in unit of pixel. |
| width | int | Represents the width of Button, in unit of pixel. |

**Returns:** A Button object.

### addLabel(topRow, top, leftColumn, left, height, width) {#addlabel}

Adds a Label to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of Label from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of Label from its left column, in unit of pixel. |
| height | int | Represents the height of Label, in unit of pixel. |
| width | int | Represents the width of Label, in unit of pixel. |

**Returns:** A Label object.

### addLabelInChart(top, left, height, width) {#addlabelinchart}

Adds a label to the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| top | int | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of label, in units of 1/4000 of the chart area. |
| width | int | Represents the width of label, in units of 1/4000 of the chart area. |

**Returns:** A new Label object.

### addTextBoxInChart(top, left, height, width) {#addtextboxinchart}

Adds a textbox to the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| top | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | int | Represents the width of textbox, in units of 1/4000 of the chart area. |

**Returns:** A TextBox object.

### addTextEffectInChart(effect, text, fontName, size, fontBold, fontItalic, top, left, height, width) {#addtexteffectinchart}

Inserts a WordArt object to the chart

| Parameter | Type | Description |
| --- | --- | --- |
| effect | int | A MsoPresetTextEffect value. The mso preset text effect type. |
| text | String | The WordArt text. |
| fontName | String | The font name. |
| size | int | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| top | int | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of shape, in units of 1/4000 of the chart area. |
| width | int | Represents the width of shape, in units of 1/4000 of the chart area. |

**Returns:** Returns a Shape object that represents the new WordArt object.

### addTextEffect(effect, text, fontName, size, fontBold, fontItalic, topRow, top, leftColumn, left, height, width) {#addtexteffect}

Inserts a WordArt object.

| Parameter | Type | Description |
| --- | --- | --- |
| effect | int | A MsoPresetTextEffect value. The mso preset text effect type. |
| text | String | The WordArt text. |
| fontName | String | The font name. |
| size | int | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int | Represents the height of shape, in unit of pixel. |
| width | int | Represents the width of shape, in unit of pixel. |

**Returns:** Returns a Shape object that represents the new WordArt object.

### addWordArt(style, text, topRow, top, leftColumn, left, height, width) {#addwordart}

Adds preset WordArt since Excel 2007.s

| Parameter | Type | Description |
| --- | --- | --- |
| style | int | A PresetWordArtStyle value. The preset WordArt Style. |
| text | String | The text. |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int | Represents the height of shape, in unit of pixel. |
| width | int | Represents the width of shape, in unit of pixel. |

### addRectangle(topRow, top, leftColumn, left, height, width) {#addrectangle}

Adds a RectangleShape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of RectangleShape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of RectangleShape from its left column, in unit of pixel. |
| height | int | Represents the height of RectangleShape, in unit of pixel. |
| width | int | Represents the width of RectangleShape, in unit of pixel. |

**Returns:** A RectangleShape object.

### addOval(topRow, top, leftColumn, left, height, width) {#addoval}

Adds a Oval to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of Oval from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of Oval from its left column, in unit of pixel. |
| height | int | Represents the height of Oval, in unit of pixel. |
| width | int | Represents the width of Oval, in unit of pixel. |

**Returns:** A Oval object.

### addLine(topRow, top, leftColumn, left, height, width) {#addline}

Adds a LineShape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of LineShape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of LineShape from its left column, in unit of pixel. |
| height | int | Represents the height of LineShape, in unit of pixel. |
| width | int | Represents the width of LineShape, in unit of pixel. |

**Returns:** A LineShape object.

### addFreeFloatingShape(type, top, left, height, width, imageData, isOriginalSize) {#addfreefloatingshape}

Adds a free floating shape to the worksheet.Only applies for line/image shape.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A MsoDrawingType value. The shape type. |
| top | int | Represents the vertical offset of shape from the worksheet's top row, in unit of pixel. |
| left | int | Represents the horizontal offset of shape from the worksheet's left column, in unit of pixel. |
| height | int | Represents the height of LineShape, in unit of pixel. |
| width | int | Represents the width of LineShape, in unit of pixel. |
| imageData | byte[] | The image data,only applies for the picture. |
| isOriginalSize | boolean | Whether the shape use original size if the shape is image. |

### addShapeInChart(type, placement, left, top, right, bottom, imageData) (1 of 2) {#addshapeinchart}

Add a shape to chart .All unit is 1/4000 of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A MsoDrawingType value. The drawing type. |
| placement | int | A PlacementType value. the placement type. |
| left | int | In unit of 1/4000 chart area width. |
| top | int | In unit of 1/4000 chart area height. |
| right | int | In unit of 1/4000 chart area width. |
| bottom | int | In unit of 1/4000 chart area height. |
| imageData | byte[] | If the shape is not a picture or ole object,imageData should be null. |

---

### addShapeInChart(type, placement, left, top, right, bottom) (2 of 2) {#addshapeinchart-1}

Add a shape to chart .All unit is 1/4000 of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A MsoDrawingType value. The drawing type. |
| placement | int | A PlacementType value. the placement type. |
| left | int | In unit of 1/4000 chart area width. |
| top | int | In unit of 1/4000 chart area height. |
| right | int | In unit of 1/4000 chart area width. |
| bottom | int | In unit of 1/4000 chart area height. |

### addShapeInChartByScale(type, placement, left, top, right, bottom) (1 of 2) {#addshapeinchartbyscale}

Add a shape to chart. All unit is percent scale of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A MsoDrawingType value. The drawing type. |
| placement | int | A PlacementType value. the placement type. |
| left | float | Unit is percent scale of chart area width. |
| top | float | Unit is percent scale of chart area height. |
| right | float | Unit is percent scale of chart area width. |
| bottom | float | Unit is percent scale of chart area height. |

---

### addShapeInChartByScale(type, placement, left, top, right, bottom, imageData) (2 of 2) {#addshapeinchartbyscale-1}

Add a shape to chart .All unit is 1/4000 of chart area.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A MsoDrawingType value. The drawing type. |
| placement | int | A PlacementType value. the placement type. |
| left | float | Unit is percent scale of chart area width. |
| top | float | Unit is percent scale of chart area height. |
| right | float | Unit is percent scale of chart area width. |
| bottom | float | Unit is percent scale of chart area height. |
| imageData | byte[] | If the shape is not a picture or ole object,imageData should be null. |

### addArc(topRow, top, leftColumn, left, height, width) {#addarc}

Adds a ArcShape to the worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of ArcShape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of ArcShape from its left column, in unit of pixel. |
| height | int | Represents the height of ArcShape, in unit of pixel. |
| width | int | Represents the width of ArcShape, in unit of pixel. |

**Returns:** A ArcShape object.

### addShape(type, topRow, top, leftColumn, left, height, width) {#addshape}

Adds a Shape to the worksheet.

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A MsoDrawingType value. Mso drawing type. |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |

**Returns:** A Shape object.

### addAutoShape(type, topRow, top, leftColumn, left, height, width) {#addautoshape}

Adds a AutoShape to the worksheet.

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A AutoShapeType value. Auto shape type. |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |

**Returns:** A Shape object.

### addAutoShapeInChart(type, top, left, height, width) {#addautoshapeinchart}

Adds a AutoShape to the chart.

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A AutoShapeType value. Auto shape type. |
| top | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | int | Represents the width of textbox, in units of 1/4000 of the chart area. |

**Returns:** Returns a shape object.

### addActiveXControl(type, topRow, top, leftColumn, left, width, height) {#addactivexcontrol}

Creates an Activex Control.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ControlType value. The type of the control. |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |

### addSvg(topRow, top, leftColumn, left, height, width, svgData, compatibleImageData) {#addsvg}

Adds svg image.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | The horizontal offset of shape from its left column, in unit of pixel. |
| height | int | The height of shape, in unit of pixel. |
| width | int | The width of shape, in unit of pixel. |
| svgData | byte[] | The svg image data. |
| compatibleImageData | byte[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

### addIcons(topRow, top, leftColumn, left, height, width, imageByteData, compatibleImageData) {#addicons}

Adds svg image.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn |  | Upper left column index. |
| left | int | The horizontal offset of shape from its left column, in unit of pixel. |
| height | int | The height of shape, in unit of pixel. |
| width | int | The width of shape, in unit of pixel. |
| imageByteData | byte[] | The image byte data. |
| compatibleImageData | byte[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

### addLinkedPicture(topRow, leftColumn, height, width, sourceFullName) {#addlinkedpicture}

Add a linked picture.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | int | The height of the shape. In unit of pixels |
| width | int | The width of the shape. In unit of pixels |
| sourceFullName | String | The path and name of the source file for the linked image |

**Returns:** Picture Picture object.

### addOleObjectWithLinkedImage(topRow, leftColumn, height, width, sourceFullName) {#addoleobjectwithlinkedimage}

Add a linked picture.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| height | int | The height of the shape. In unit of pixels |
| width | int | The width of the shape. In unit of pixels |
| sourceFullName | String | The path and name of the source file for the linked image |

**Returns:** Picture Picture object.

### addOleObject(topRow, top, leftColumn, left, height, width, imageData) {#addoleobject}

Adds an OleObject.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  |  |
| top | int |  |
| upperLeftColumn |  |  |
| left | int |  |
| height | int |  |
| width | int |  |
| imageData | byte[] |  |

### copyCommentsInRange(shapes, ca, destRow, destColumn) {#copycommentsinrange}

Copy all comments in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| shapes | ShapeCollection | The source shapes. |
| ca | CellArea | The source range. |
| destRow | int | The dest range start row. |
| destColumn | int | The dest range start column. |

### copyInRange(sourceShapes, ca, destRow, destColumn, isContained) {#copyinrange}

Copy shapes in the range to destination range.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Source shapes. |
| ca | CellArea | The source range. |
| destRow | int | The dest row index of the dest range. |
| destColumn | int | The dest column of the dest range. |
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

### group(groupItems) {#group}

Group the shapes.

The shape in the groupItems should not be grouped. The shape must be in this Shapes collection.

| Parameter | Type | Description |
| --- | --- | --- |
| groupItems | Shape[] | the group items. |

**Returns:** Return the group shape.

### ungroup(group) {#ungroup}

Ungroups the shape items.

If the group shape is grouped by another group shape,nothing will be done.

| Parameter | Type | Description |
| --- | --- | --- |
| group | GroupShape | The group shape. |

### removeAt(index) {#removeat}

Remove the shape.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the shape. |

### remove(shape) {#remove}

Remove the shape.

| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape |  |

### clear() {#clear}

Clear all shapes in the worksheet.

### updateSelectedValue() {#updateselectedvalue}

Update the selected value by the value of the linked cell or range of the shape.

### addFreeform(topRow, top, leftColumn, left, height, width, paths) {#addfreeform}

### addSignatureLine(topRow, leftColumn, signatureLine) {#addsignatureline}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.

### addPictureFromBytes(upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn, byte_array) (1 of 2) {#addpicturefrombytes}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index |
| upperLeftColumn | int | Upper left column index |
| lowerRightRow | int | Lower right row index |
| lowerRightColumn | int | Lower right column index |
| byte_array | bytes | The byte array |

**Returns:** Returns a Picture objct

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook(FileFormatType.XLSX)
with open('cells.png', 'rb') as pic:
    pic_bytes = pic.read()
    wb.getWorksheets().get(0).getShapes().addPictureFromBytes(2, 7, lowerRightRow=10, lowerRightColumn=10, byte_array=pic_bytes)
wb.save("wb.xlsx")

jpype.shutdownJVM()
```

---

### addPictureFromBytes(upperLeftRow, upperLeftColumn, byte_array, widthScale, heightScale) (2 of 2) {#addpicturefrombytes-1}

Adds a picture to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index |
| upperLeftColumn | int | Upper left column index |
| byte_array | bytes | The byte array |
| widthScale | int | Scale of image width, a percentage |
| heightScale | int | Scale of image height, a percentage |

**Returns:** Returns a Picture objct

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook(FileFormatType.XLSX)
with open('cells.png', 'rb') as pic:
    pic_bytes = pic.read()
    wb.getWorksheets().get(0).getShapes().addPictureFromBytes(2, 0, byte_array=pic_bytes, widthScale=200, heightScale=150)
wb.save("wb.xlsx")

jpype.shutdownJVM()
```

### addPictureInChartFromBytes(top, left, byte_array, widthScale, heightScale) {#addpictureinchartfrombytes}

Adds a picture to the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| top | int | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area |
| left | int | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area |
| byte_array | bytes | The byte array |
| widthScale | int | Scale of image width, a percentage |
| heightScale | int | Scale of image height, a percentage |

**Returns:** Returns a Picture objct

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook('Book2.xlsx')
shapes = wb.getWorksheets().get("Chart").getCharts().get(0).getShapes()
with open('cells.png', 'rb') as pic:
    picture = shapes.addPictureInChartFromBytes(1, 1, pic.read(), 10, 5)
wb.save("wb.xlsx")

jpype.shutdownJVM()
```
