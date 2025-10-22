##ShapeCollection
Represents all the shape in a worksheetchart.
## ShapeCollection class
Represents all the shape in a worksheet/chart.
```javascript
class ShapeCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Shape](../shape/) object at the specific index in the list. |
| [get(string)](#get-string-)| Gets the [Shape](../shape/) object by the name of the shape. |
| [addCopy(Shape, number, number, number, number)](#addCopy-shape-number-number-number-number-)| Adds and copy a shape to the worksheet. |
| [addCheckBox(number, number, number, number, number, number)](#addCheckBox-number-number-number-number-number-number-)| Adds a checkbox to the worksheet. |
| [addTextBox(number, number, number, number, number, number)](#addTextBox-number-number-number-number-number-number-)| Adds a text box to the worksheet. |
| [addEquation(number, number, number, number, number, number)](#addEquation-number-number-number-number-number-number-)| Add an equation object to the worksheet. |
| [addSpinner(number, number, number, number, number, number)](#addSpinner-number-number-number-number-number-number-)| Adds a Spinner to the worksheet. |
| [addScrollBar(number, number, number, number, number, number)](#addScrollBar-number-number-number-number-number-number-)| Adds a ScrollBar to the worksheet. |
| [addRadioButton(number, number, number, number, number, number)](#addRadioButton-number-number-number-number-number-number-)| Adds a RadioButton to the worksheet. |
| [addListBox(number, number, number, number, number, number)](#addListBox-number-number-number-number-number-number-)| Adds a ListBox to the worksheet. |
| [addComboBox(number, number, number, number, number, number)](#addComboBox-number-number-number-number-number-number-)| Adds a ComboBox to the worksheet. |
| [addGroupBox(number, number, number, number, number, number)](#addGroupBox-number-number-number-number-number-number-)| Adds a GroupBox to the worksheet. |
| [addButton(number, number, number, number, number, number)](#addButton-number-number-number-number-number-number-)| Adds a Button to the worksheet. |
| [addLabel(number, number, number, number, number, number)](#addLabel-number-number-number-number-number-number-)| Adds a Label to the worksheet. |
| [addLabelInChart(number, number, number, number)](#addLabelInChart-number-number-number-number-)| Adds a label to the chart. |
| [addTextBoxInChart(number, number, number, number)](#addTextBoxInChart-number-number-number-number-)| Adds a textbox to the chart. |
| [addTextEffectInChart(MsoPresetTextEffect, string, string, number, boolean, boolean, number, number, number, number)](#addTextEffectInChart-msopresettexteffect-string-string-number-boolean-boolean-number-number-number-number-)| Inserts a WordArt object to the chart |
| [addTextEffect(MsoPresetTextEffect, string, string, number, boolean, boolean, number, number, number, number, number, number)](#addTextEffect-msopresettexteffect-string-string-number-boolean-boolean-number-number-number-number-number-number-)| Inserts a WordArt object. |
| [addWordArt(PresetWordArtStyle, string, number, number, number, number, number, number)](#addWordArt-presetwordartstyle-string-number-number-number-number-number-number-)| Adds preset WordArt since Excel 2007.s |
| [addRectangle(number, number, number, number, number, number)](#addRectangle-number-number-number-number-number-number-)| Adds a RectangleShape to the worksheet. |
| [addOval(number, number, number, number, number, number)](#addOval-number-number-number-number-number-number-)| Adds a Oval to the worksheet. |
| [addLine(number, number, number, number, number, number)](#addLine-number-number-number-number-number-number-)| Adds a LineShape to the worksheet. |
| [addFreeFloatingShape(MsoDrawingType, number, number, number, number, Uint8Array, boolean)](#addFreeFloatingShape-msodrawingtype-number-number-number-number-uint8array-boolean-)| Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [addShapeInChart(MsoDrawingType, PlacementType, number, number, number, number, Uint8Array)](#addShapeInChart-msodrawingtype-placementtype-number-number-number-number-uint8array-)| Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChart(MsoDrawingType, PlacementType, number, number, number, number)](#addShapeInChart-msodrawingtype-placementtype-number-number-number-number-)| Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChartByScale(MsoDrawingType, PlacementType, number, number, number, number)](#addShapeInChartByScale-msodrawingtype-placementtype-number-number-number-number-)| Add a shape to chart. All unit is percent scale of chart area. |
| [addShapeInChartByScale(MsoDrawingType, PlacementType, number, number, number, number, Uint8Array)](#addShapeInChartByScale-msodrawingtype-placementtype-number-number-number-number-uint8array-)| Add a shape to chart .All unit is 1/4000 of chart area. |
| [addArc(number, number, number, number, number, number)](#addArc-number-number-number-number-number-number-)| Adds a ArcShape to the worksheet. |
| [addShape(MsoDrawingType, number, number, number, number, number, number)](#addShape-msodrawingtype-number-number-number-number-number-number-)| Adds a Shape to the worksheet. |
| [addAutoShape(AutoShapeType, number, number, number, number, number, number)](#addAutoShape-autoshapetype-number-number-number-number-number-number-)| Adds a AutoShape to the worksheet. |
| [addAutoShapeInChart(AutoShapeType, number, number, number, number)](#addAutoShapeInChart-autoshapetype-number-number-number-number-)| Adds a AutoShape to the chart. |
| [addActiveXControl(ControlType, number, number, number, number, number, number)](#addActiveXControl-controltype-number-number-number-number-number-number-)| Creates an Activex Control. |
| [addPicture(number, number, number, number, Uint8Array)](#addPicture-number-number-number-number-uint8array-)| Adds a picture to the collection. |
| [addPicture(number, number, Uint8Array, number, number)](#addPicture-number-number-uint8array-number-number-)| Adds a picture to the collection. |
| [addSvg(number, number, number, number, number, number, Uint8Array, Uint8Array)](#addSvg-number-number-number-number-number-number-uint8array-uint8array-)| Adds svg image. |
| [addIcons(number, number, number, number, number, number, Uint8Array, Uint8Array)](#addIcons-number-number-number-number-number-number-uint8array-uint8array-)| Adds svg image. |
| [addLinkedPicture(number, number, number, number, string)](#addLinkedPicture-number-number-number-number-string-)| Add a linked picture. |
| [addOleObjectWithLinkedImage(number, number, number, number, string)](#addOleObjectWithLinkedImage-number-number-number-number-string-)| Add a linked picture. |
| [addPictureInChart(number, number, Uint8Array, number, number)](#addPictureInChart-number-number-uint8array-number-number-)| Adds a picture to the chart. |
| [addOleObject(number, number, number, number, number, number, Uint8Array)](#addOleObject-number-number-number-number-number-number-uint8array-)| Adds an OleObject. |
| [copyCommentsInRange(ShapeCollection, CellArea, number, number)](#copyCommentsInRange-shapecollection-cellarea-number-number-)| Copy all comments in the range. |
| [copyInRange(ShapeCollection, CellArea, number, number, boolean)](#copyInRange-shapecollection-cellarea-number-number-boolean-)| Copy shapes in the range to destination range. |
| [deleteInRange(CellArea)](#deleteInRange-cellarea-)| Delete shapes in the range.Comment shapes will not be deleted. |
| [deleteShape(Shape)](#deleteShape-shape-)| Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. |
| [group(Shape[])](#group-shapearray-)| Group the shapes. |
| [ungroup(GroupShape)](#ungroup-groupshape-)| Ungroups the shape items. |
| [removeAt(number)](#removeAt-number-)| Remove the shape. |
| [remove(Shape)](#remove-shape-)| Remove the shape. |
| [clear()](#clear--)| Clear all shapes in the worksheet. |
| [updateSelectedValue()](#updateSelectedValue--)| Update the selected value by the value of the linked cell or range of the shape. |
| [addFreeform(number, number, number, number, number, number, ShapePath[])](#addFreeform-number-number-number-number-number-number-shapepatharray-)| Adds a freeform shape to the worksheet. |
| [addSignatureLine(number, number, SignatureLine)](#addSignatureLine-number-number-signatureline-)| Adds a Signature Line to the worksheet. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [Shape](../shape/) object at the specific index in the list.
```javascript
get(index: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[Shape](../shape/)
### get(string) {#get-string-}
Gets the [Shape](../shape/) object by the name of the shape.
```javascript
get(name: string) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the shape. |
**Returns**
[Shape](../shape/)
### addCopy(Shape, number, number, number, number) {#addCopy-shape-number-number-number-number-}
Adds and copy a shape to the worksheet.
```javascript
addCopy(sourceShape: Shape, topRow: number, top: number, leftColumn: number, left: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | [Shape](../shape/) | Source shape. |
| topRow | number | The top row index. |
| top | number | Represents the vertical  offset from its top row, in unit of pixel. |
| leftColumn | number | The left column index. |
| left | number | Represents the horizontal offset from its left column, in unit of pixel. |
**Returns**
The new [Shape](../shape/) object.
### addCheckBox(number, number, number, number, number, number) {#addCheckBox-number-number-number-number-number-number-}
Adds a checkbox to the worksheet.
```javascript
addCheckBox(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : CheckBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of checkbox from its top row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | number | Height of textbox, in unit of pixel. |
| width | number | Width of textbox, in unit of pixel. |
**Returns**
The new CheckBox object index.
### addTextBox(number, number, number, number, number, number) {#addTextBox-number-number-number-number-number-number-}
Adds a text box to the worksheet.
```javascript
addTextBox(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : TextBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of textbox from its top row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | number | Represents the height of textbox, in unit of pixel. |
| width | number | Represents the width of textbox, in unit of pixel. |
**Returns**
A [TextBox](../textbox/) object.
### addEquation(number, number, number, number, number, number) {#addEquation-number-number-number-number-number-number-}
Add an equation object to the worksheet.
```javascript
addEquation(topRow: number, top: number, leftColumn: number, left: number, height: number, width: number) : TextBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | The top row index. |
| top | number | The vertical  offset its top row, in unit of pixel. |
| leftColumn | number | The left column index. |
| left | number | The horizontal offset from its left column, in unit of pixel. |
| height | number | The height of equation, in unit of pixel. |
| width | number | The width of equation, in unit of pixel. |
**Returns**
[TextBox](../textbox/)
### addSpinner(number, number, number, number, number, number) {#addSpinner-number-number-number-number-number-number-}
Adds a Spinner to the worksheet.
```javascript
addSpinner(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Spinner;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of Spinner from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of Spinner from its left column, in unit of pixel. |
| height | number | Represents the height of Spinner, in unit of pixel. |
| width | number | Represents the width of Spinner, in unit of pixel. |
**Returns**
A Spinner object.
### addScrollBar(number, number, number, number, number, number) {#addScrollBar-number-number-number-number-number-number-}
Adds a ScrollBar to the worksheet.
```javascript
addScrollBar(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : ScrollBar;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of ScrollBar from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of ScrollBar from its left column, in unit of pixel. |
| height | number | Represents the height of ScrollBar, in unit of pixel. |
| width | number | Represents the width of ScrollBar, in unit of pixel. |
**Returns**
A ScrollBar object.
### addRadioButton(number, number, number, number, number, number) {#addRadioButton-number-number-number-number-number-number-}
Adds a RadioButton to the worksheet.
```javascript
addRadioButton(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : RadioButton;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of RadioButton from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of RadioButton from its left column, in unit of pixel. |
| height | number | Represents the height of RadioButton, in unit of pixel. |
| width | number | Represents the width of RadioButton, in unit of pixel. |
**Returns**
A RadioButton object.
### addListBox(number, number, number, number, number, number) {#addListBox-number-number-number-number-number-number-}
Adds a ListBox to the worksheet.
```javascript
addListBox(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : ListBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of ListBox from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of ListBox from its left column, in unit of pixel. |
| height | number | Represents the height of ListBox, in unit of pixel. |
| width | number | Represents the width of ListBox, in unit of pixel. |
**Returns**
A ListBox object.
### addComboBox(number, number, number, number, number, number) {#addComboBox-number-number-number-number-number-number-}
Adds a ComboBox to the worksheet.
```javascript
addComboBox(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : ComboBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of ComboBox from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of ComboBox from its left column, in unit of pixel. |
| height | number | Represents the height of ComboBox, in unit of pixel. |
| width | number | Represents the width of ComboBox, in unit of pixel. |
**Returns**
A ComboBox object.
### addGroupBox(number, number, number, number, number, number) {#addGroupBox-number-number-number-number-number-number-}
Adds a GroupBox to the worksheet.
```javascript
addGroupBox(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : GroupBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of GroupBox from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of GroupBox from its left column, in unit of pixel. |
| height | number | Represents the height of GroupBox, in unit of pixel. |
| width | number | Represents the width of GroupBox, in unit of pixel. |
**Returns**
A GroupBox object.
### addButton(number, number, number, number, number, number) {#addButton-number-number-number-number-number-number-}
Adds a Button to the worksheet.
```javascript
addButton(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Button;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of Button from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of Button from its left column, in unit of pixel. |
| height | number | Represents the height of Button, in unit of pixel. |
| width | number | Represents the width of Button, in unit of pixel. |
**Returns**
A Button object.
### addLabel(number, number, number, number, number, number) {#addLabel-number-number-number-number-number-number-}
Adds a Label to the worksheet.
```javascript
addLabel(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Label;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of Label from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of Label from its left column, in unit of pixel. |
| height | number | Represents the height of Label, in unit of pixel. |
| width | number | Represents the width of Label, in unit of pixel. |
**Returns**
A Label object.
### addLabelInChart(number, number, number, number) {#addLabelInChart-number-number-number-number-}
Adds a label to the chart.
```javascript
addLabelInChart(top: number, left: number, height: number, width: number) : Label;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| top | number | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| left | number | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| height | number | Represents the height of label, in units of 1/4000 of the chart area. |
| width | number | Represents the width of label, in units of 1/4000 of the chart area. |
**Returns**
A new Label object.
### addTextBoxInChart(number, number, number, number) {#addTextBoxInChart-number-number-number-number-}
Adds a textbox to the chart.
```javascript
addTextBoxInChart(top: number, left: number, height: number, width: number) : TextBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| top | number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | number | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | number | Represents the width of textbox, in units of 1/4000 of the chart area. |
**Returns**
A TextBox object.
### addTextEffectInChart(MsoPresetTextEffect, string, string, number, boolean, boolean, number, number, number, number) {#addTextEffectInChart-msopresettexteffect-string-string-number-boolean-boolean-number-number-number-number-}
Inserts a WordArt object to the chart
```javascript
addTextEffectInChart(effect: MsoPresetTextEffect, text: string, fontName: string, size: number, fontBold: boolean, fontItalic: boolean, top: number, left: number, height: number, width: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| effect | [MsoPresetTextEffect](../msopresettexteffect/) | The mso preset text effect type. |
| text | string | The WordArt text. |
| fontName | string | The font name. |
| size | number | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| top | number | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | number | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| height | number | Represents the height of shape, in units of 1/4000 of the chart area. |
| width | number | Represents the width of shape, in units of 1/4000 of the chart area. |
**Returns**
Returns a Shape object that represents the new WordArt object.
### addTextEffect(MsoPresetTextEffect, string, string, number, boolean, boolean, number, number, number, number, number, number) {#addTextEffect-msopresettexteffect-string-string-number-boolean-boolean-number-number-number-number-number-number-}
Inserts a WordArt object.
```javascript
addTextEffect(effect: MsoPresetTextEffect, text: string, fontName: string, size: number, fontBold: boolean, fontItalic: boolean, upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| effect | [MsoPresetTextEffect](../msopresettexteffect/) | The mso preset text effect type. |
| text | string | The WordArt text. |
| fontName | string | The font name. |
| size | number | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | number | Represents the height of shape, in unit of pixel. |
| width | number | Represents the width of shape, in unit of pixel. |
**Returns**
Returns a Shape object that represents the new WordArt object.
### addWordArt(PresetWordArtStyle, string, number, number, number, number, number, number) {#addWordArt-presetwordartstyle-string-number-number-number-number-number-number-}
Adds preset WordArt since Excel 2007.s
```javascript
addWordArt(style: PresetWordArtStyle, text: string, upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](../presetwordartstyle/) | The preset WordArt Style. |
| text | string | The text. |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | number | Represents the height of shape, in unit of pixel. |
| width | number | Represents the width of shape, in unit of pixel. |
**Returns**
[Shape](../shape/)
### addRectangle(number, number, number, number, number, number) {#addRectangle-number-number-number-number-number-number-}
Adds a RectangleShape to the worksheet.
```javascript
addRectangle(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : RectangleShape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of RectangleShape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of RectangleShape from its left column, in unit of pixel. |
| height | number | Represents the height of RectangleShape, in unit of pixel. |
| width | number | Represents the width of RectangleShape, in unit of pixel. |
**Returns**
A RectangleShape object.
### addOval(number, number, number, number, number, number) {#addOval-number-number-number-number-number-number-}
Adds a Oval to the worksheet.
```javascript
addOval(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Oval;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of Oval from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of Oval from its left column, in unit of pixel. |
| height | number | Represents the height of Oval, in unit of pixel. |
| width | number | Represents the width of Oval, in unit of pixel. |
**Returns**
A Oval object.
### addLine(number, number, number, number, number, number) {#addLine-number-number-number-number-number-number-}
Adds a LineShape to the worksheet.
```javascript
addLine(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : LineShape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of LineShape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of LineShape from its left column, in unit of pixel. |
| height | number | Represents the height of LineShape, in unit of pixel. |
| width | number | Represents the width of LineShape, in unit of pixel. |
**Returns**
A LineShape object.
### addFreeFloatingShape(MsoDrawingType, number, number, number, number, Uint8Array, boolean) {#addFreeFloatingShape-msodrawingtype-number-number-number-number-uint8array-boolean-}
Adds a free floating shape to the worksheet.Only applies for line/image shape.
```javascript
addFreeFloatingShape(type: MsoDrawingType, top: number, left: number, height: number, width: number, imageData: Uint8Array, isOriginalSize: boolean) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [MsoDrawingType](../msodrawingtype/) | The shape type. |
| top | number | Represents the vertical  offset of shape from the worksheet's top row, in unit of pixel. |
| left | number | Represents the horizontal offset of shape from the worksheet's left column, in unit of pixel. |
| height | number | Represents the height of LineShape, in unit of pixel. |
| width | number | Represents the width of LineShape, in unit of pixel. |
| imageData | number[] | The image data,only applies for the picture. |
| isOriginalSize | boolean | Whether the shape use original size if the shape is image. |
**Returns**
[Shape](../shape/)
### addShapeInChart(MsoDrawingType, PlacementType, number, number, number, number, Uint8Array) {#addShapeInChart-msodrawingtype-placementtype-number-number-number-number-uint8array-}
Add a shape to chart .All unit is 1/4000 of chart area.
```javascript
addShapeInChart(type: MsoDrawingType, placement: PlacementType, left: number, top: number, right: number, bottom: number, imageData: Uint8Array) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [MsoDrawingType](../msodrawingtype/) | The drawing type. |
| placement | [PlacementType](../placementtype/) | the placement type. |
| left | number | In unit of 1/4000 chart area width. |
| top | number | In unit of 1/4000 chart area height. |
| right | number | In unit of 1/4000 chart area width. |
| bottom | number | In unit of 1/4000 chart area height. |
| imageData | number[] | If the shape is not a picture or ole object,imageData should be null. |
**Returns**
[Shape](../shape/)
### addShapeInChart(MsoDrawingType, PlacementType, number, number, number, number) {#addShapeInChart-msodrawingtype-placementtype-number-number-number-number-}
Add a shape to chart .All unit is 1/4000 of chart area.
```javascript
addShapeInChart(type: MsoDrawingType, placement: PlacementType, left: number, top: number, right: number, bottom: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [MsoDrawingType](../msodrawingtype/) | The drawing type. |
| placement | [PlacementType](../placementtype/) | the placement type. |
| left | number | In unit of 1/4000 chart area width. |
| top | number | In unit of 1/4000 chart area height. |
| right | number | In unit of 1/4000 chart area width. |
| bottom | number | In unit of 1/4000 chart area height. |
**Returns**
[Shape](../shape/)
### addShapeInChartByScale(MsoDrawingType, PlacementType, number, number, number, number) {#addShapeInChartByScale-msodrawingtype-placementtype-number-number-number-number-}
Add a shape to chart. All unit is percent scale of chart area.
```javascript
addShapeInChartByScale(type: MsoDrawingType, placement: PlacementType, left: number, top: number, right: number, bottom: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [MsoDrawingType](../msodrawingtype/) | The drawing type. |
| placement | [PlacementType](../placementtype/) | the placement type. |
| left | number | Unit is percent scale of chart area width. |
| top | number | Unit is percent scale of chart area height. |
| right | number | Unit is percent scale of chart area width. |
| bottom | number | Unit is percent scale of chart area height. |
**Returns**
[Shape](../shape/)
### addShapeInChartByScale(MsoDrawingType, PlacementType, number, number, number, number, Uint8Array) {#addShapeInChartByScale-msodrawingtype-placementtype-number-number-number-number-uint8array-}
Add a shape to chart .All unit is 1/4000 of chart area.
```javascript
addShapeInChartByScale(type: MsoDrawingType, placement: PlacementType, left: number, top: number, right: number, bottom: number, imageData: Uint8Array) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [MsoDrawingType](../msodrawingtype/) | The drawing type. |
| placement | [PlacementType](../placementtype/) | the placement type. |
| left | number | Unit is percent scale of chart area width. |
| top | number | Unit is percent scale of chart area height. |
| right | number | Unit is percent scale of chart area width. |
| bottom | number | Unit is percent scale of chart area height. |
| imageData | number[] | If the shape is not a picture or ole object,imageData should be null. |
**Returns**
[Shape](../shape/)
### addArc(number, number, number, number, number, number) {#addArc-number-number-number-number-number-number-}
Adds a ArcShape to the worksheet.
```javascript
addArc(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : ArcShape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of ArcShape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of ArcShape from its left column, in unit of pixel. |
| height | number | Represents the height of ArcShape, in unit of pixel. |
| width | number | Represents the width of ArcShape, in unit of pixel. |
**Returns**
A ArcShape object.
### addShape(MsoDrawingType, number, number, number, number, number, number) {#addShape-msodrawingtype-number-number-number-number-number-number-}
Adds a Shape to the worksheet.
```javascript
addShape(type: MsoDrawingType, upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [MsoDrawingType](../msodrawingtype/) | Mso drawing type. |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | number | Represents the height of Shape, in unit of pixel. |
| width | number | Represents the width of Shape, in unit of pixel. |
**Returns**
A Shape object.
**Remarks**
The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox
### addAutoShape(AutoShapeType, number, number, number, number, number, number) {#addAutoShape-autoshapetype-number-number-number-number-number-number-}
Adds a AutoShape to the worksheet.
```javascript
addAutoShape(type: AutoShapeType, upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [AutoShapeType](../autoshapetype/) | Auto shape type. |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | number | Represents the height of Shape, in unit of pixel. |
| width | number | Represents the width of Shape, in unit of pixel. |
**Returns**
A Shape object.
**Remarks**
The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox
### addAutoShapeInChart(AutoShapeType, number, number, number, number) {#addAutoShapeInChart-autoshapetype-number-number-number-number-}
Adds a AutoShape to the chart.
```javascript
addAutoShapeInChart(type: AutoShapeType, top: number, left: number, height: number, width: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [AutoShapeType](../autoshapetype/) | Auto shape type. |
| top | number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | number | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | number | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | number | Represents the width of textbox, in units of 1/4000 of the chart area. |
**Returns**
Returns a shape object.
**Remarks**
The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox
### addActiveXControl(ControlType, number, number, number, number, number, number) {#addActiveXControl-controltype-number-number-number-number-number-number-}
Creates an Activex Control.
```javascript
addActiveXControl(type: ControlType, topRow: number, top: number, leftColumn: number, left: number, width: number, height: number) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ControlType](../controltype/) | The type of the control. |
| topRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of Shape from its left row, in unit of pixel. |
| leftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| width | number | Represents the width of Shape, in unit of pixel. |
| height | number | Represents the height of Shape, in unit of pixel. |
**Returns**
[Shape](../shape/)
### addPicture(number, number, number, number, Uint8Array) {#addPicture-number-number-number-number-uint8array-}
Adds a picture to the collection.
```javascript
addPicture(upperLeftRow: number, upperLeftColumn: number, lowerRightRow: number, lowerRightColumn: number, stream: Uint8Array) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| lowerRightRow | number | Lower right row index |
| lowerRightColumn | number | Lower right column index |
| stream | Uint8Array | Stream object which contains the image data. |
**Returns**
[Picture](../picture/) Picture object.
### addPicture(number, number, Uint8Array, number, number) {#addPicture-number-number-uint8array-number-number-}
Adds a picture to the collection.
```javascript
addPicture(upperLeftRow: number, upperLeftColumn: number, stream: Uint8Array, widthScale: number, heightScale: number) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| stream | Uint8Array | Stream object which contains the image data. |
| widthScale | number | Scale of image width, a percentage. |
| heightScale | number | Scale of image height, a percentage. |
**Returns**
[Picture](../picture/) Picture object.
### addSvg(number, number, number, number, number, number, Uint8Array, Uint8Array) {#addSvg-number-number-number-number-number-number-uint8array-uint8array-}
Adds svg image.
```javascript
addSvg(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number, svgData: Uint8Array, compatibleImageData: Uint8Array) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | The horizontal offset of shape from its left column, in unit of pixel. |
| height | number | The height of shape, in unit of pixel. |
| width | number | The width of shape, in unit of pixel. |
| svgData | number[] | The svg image data. |
| compatibleImageData | number[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |
**Returns**
[Picture](../picture/)
### addIcons(number, number, number, number, number, number, Uint8Array, Uint8Array) {#addIcons-number-number-number-number-number-number-uint8array-uint8array-}
Adds svg image.
```javascript
addIcons(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number, imageByteData: Uint8Array, compatibleImageData: Uint8Array) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | The horizontal offset of shape from its left column, in unit of pixel. |
| height | number | The height of shape, in unit of pixel. |
| width | number | The width of shape, in unit of pixel. |
| imageByteData | number[] | The image byte data. |
| compatibleImageData | number[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |
**Returns**
[Picture](../picture/)
### addLinkedPicture(number, number, number, number, string) {#addLinkedPicture-number-number-number-number-string-}
Add a linked picture.
```javascript
addLinkedPicture(upperLeftRow: number, upperLeftColumn: number, height: number, width: number, sourceFullName: string) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| height | number | The height of the shape. In unit of pixels |
| width | number | The width of the shape. In unit of pixels |
| sourceFullName | string | The path and name of the source file for the linked image |
**Returns**
[Picture](../picture/) Picture object.
### addOleObjectWithLinkedImage(number, number, number, number, string) {#addOleObjectWithLinkedImage-number-number-number-number-string-}
Add a linked picture.
```javascript
addOleObjectWithLinkedImage(upperLeftRow: number, upperLeftColumn: number, height: number, width: number, sourceFullName: string) : OleObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| height | number | The height of the shape. In unit of pixels |
| width | number | The width of the shape. In unit of pixels |
| sourceFullName | string | The path and name of the source file for the linked image |
**Returns**
[Picture](../picture/) Picture object.
### addPictureInChart(number, number, Uint8Array, number, number) {#addPictureInChart-number-number-uint8array-number-number-}
Adds a picture to the chart.
```javascript
addPictureInChart(top: number, left: number, stream: Uint8Array, widthScale: number, heightScale: number) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| top | number | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | number | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| stream | Uint8Array | Stream object which contains the image data. |
| widthScale | number | Scale of image width, a percentage. |
| heightScale | number | Scale of image height, a percentage. |
**Returns**
Returns a Picture object.
### addOleObject(number, number, number, number, number, number, Uint8Array) {#addOleObject-number-number-number-number-number-number-uint8array-}
Adds an OleObject.
```javascript
addOleObject(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number, imageData: Uint8Array) : OleObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number |  |
| top | number |  |
| upperLeftColumn | number |  |
| left | number |  |
| height | number |  |
| width | number |  |
| imageData | number[] |  |
**Returns**
[OleObject](../oleobject/)
### copyCommentsInRange(ShapeCollection, CellArea, number, number) {#copyCommentsInRange-shapecollection-cellarea-number-number-}
Copy all comments in the range.
```javascript
copyCommentsInRange(shapes: ShapeCollection, ca: CellArea, destRow: number, destColumn: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shapes | [ShapeCollection](../shapecollection/) | The source shapes. |
| ca | [CellArea](../cellarea/) | The source range. |
| destRow | number | The dest range start row. |
| destColumn | number | The dest range start column. |
### copyInRange(ShapeCollection, CellArea, number, number, boolean) {#copyInRange-shapecollection-cellarea-number-number-boolean-}
Copy shapes in the range to destination range.
```javascript
copyInRange(sourceShapes: ShapeCollection, ca: CellArea, destRow: number, destColumn: number, isContained: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../shapecollection/) | Source shapes. |
| ca | [CellArea](../cellarea/) | The source range. |
| destRow | number | The dest row index of the dest range. |
| destColumn | number | The dest column of the dest range. |
| isContained | boolean | Whether only copy the shapes which are contained in the range.         /// If true,only copies the shapes in the range.          /// Otherwise,it works as MS Office. |
### deleteInRange(CellArea) {#deleteInRange-cellarea-}
Delete shapes in the range.Comment shapes will not be deleted.
```javascript
deleteInRange(ca: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The range.If the shapes are contained in the range, they will be removed. |
### deleteShape(Shape) {#deleteShape-shape-}
Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.
```javascript
deleteShape(shape: Shape) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shape | [Shape](../shape/) |  |
### group(Shape[]) {#group-shapearray-}
Group the shapes.
```javascript
group(groupItems: Shape[]) : GroupShape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| groupItems | [Shape](../shape/)[] | the group items. |
**Returns**
Return the group shape.
**Remarks**
The shape in the groupItems should not be grouped. The shape must be in this Shapes collection.
### ungroup(GroupShape) {#ungroup-groupshape-}
Ungroups the shape items.
```javascript
ungroup(group: GroupShape) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| group | [GroupShape](../groupshape/) | The group shape. |
**Remarks**
If the group shape is grouped by another group shape,nothing will be done.
### removeAt(number) {#removeAt-number-}
Remove the shape.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the shape. |
### remove(Shape) {#remove-shape-}
Remove the shape.
```javascript
remove(shape: Shape) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shape | [Shape](../shape/) |  |
### clear() {#clear--}
Clear all shapes in the worksheet.
```javascript
clear() : void;
```
### updateSelectedValue() {#updateSelectedValue--}
Update the selected value by the value of the linked cell or range of the shape.
```javascript
updateSelectedValue() : void;
```
### addFreeform(number, number, number, number, number, number, ShapePath[]) {#addFreeform-number-number-number-number-number-number-shapepatharray-}
Adds a freeform shape to the worksheet.
```javascript
addFreeform(upperLeftRow: number, top: number, upperLeftColumn: number, left: number, height: number, width: number, paths: ShapePath[]) : Shape;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| top | number | Represents the vertical  offset of freeform shape from its left row, in unit of pixel. |
| upperLeftColumn | number | Upper left column index. |
| left | number | Represents the horizontal offset of freeform shape from its left column, in unit of pixel. |
| height | number | Represents the height of freeform shape, in unit of pixel. |
| width | number | Represents the width of freeform shape, in unit of pixel. |
| paths | [ShapePath](../shapepath/)[] | Represents a user-defined path |
**Returns**
A freeform shape.
**Remarks**
Notice: That the width and height in the parameters can be any positive integer values, not the total width and height of the ShapePath array specified by ’paths'. The relationship between them is a scale-fill relationship, that is, each ShapePath object will be scaled according to the width and height. Therefore, when there are multiple objects in the 'paths', each ShapePath object needs to be designed reasonably to meet expectations. When there is only one ShapePath object and there are no other requirements, passing the object's width and height as parameter values ​​is a good solution.
### addSignatureLine(number, number, SignatureLine) {#addSignatureLine-number-number-signatureline-}
Adds a Signature Line to the worksheet.
```javascript
addSignatureLine(upperLeftRow: number, upperLeftColumn: number, signatureLine: SignatureLine) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| signatureLine | [SignatureLine](../signatureline/) | Represents a signature line object. |
**Returns**
[Picture](../picture/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
