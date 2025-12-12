---
title: Aspose::Cells::Drawing::ShapeCollection class
linktitle: ShapeCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection class. Represents all the shape in a worksheet/chart in C++.'
type: docs
weight: 5200
url: /cpp/aspose.cells.drawing/shapecollection/
---
## ShapeCollection class


Represents all the shape in a worksheet/chart.

```cpp
class ShapeCollection
```

## Methods

| Method | Description |
| --- | --- |
| [AddActiveXControl(ControlType type, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t width, int32_t height)](./addactivexcontrol/) | Creates an Activex Control. |
| [AddArc(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addarc/) | Adds a [ArcShape](../arcshape/) to the worksheet. |
| [AddAutoShape(AutoShapeType type, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addautoshape/) | Adds a AutoShape to the worksheet. |
| [AddAutoShapeInChart(AutoShapeType type, int32_t top, int32_t left, int32_t height, int32_t width)](./addautoshapeinchart/) | Adds a AutoShape to the chart. |
| [AddButton(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addbutton/) | Adds a [Button](../button/) to the worksheet. |
| [AddCheckBox(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addcheckbox/) | Adds a checkbox to the worksheet. |
| [AddComboBox(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addcombobox/) | Adds a [ComboBox](../combobox/) to the worksheet. |
| [AddCopy(const Shape\& sourceShape, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left)](./addcopy/) | Adds and copy a shape to the worksheet. |
| [AddEquation(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addequation/) | Adds an equation object to the worksheet. |
| [AddFreeFloatingShape(MsoDrawingType type, int32_t top, int32_t left, int32_t height, int32_t width, const Vector \<uint8_t\>\& imageData, bool isOriginalSize)](./addfreefloatingshape/) | Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [AddFreeform(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector \<ShapePath\>\& paths)](./addfreeform/) | Adds a freeform shape to the worksheet. |
| [AddGroupBox(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addgroupbox/) | Adds a [GroupBox](../groupbox/) to the worksheet. |
| [AddIcons(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector \<uint8_t\>\& imageByteData, const Vector \<uint8_t\>\& compatibleImageData)](./addicons/) | Adds svg image. |
| [AddLabel(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addlabel/) | Adds a [Label](../label/) to the worksheet. |
| [AddLabelInChart(int32_t top, int32_t left, int32_t height, int32_t width)](./addlabelinchart/) | Adds a label to the chart. |
| [AddLaTeXEquation(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const U16String\& latex)](./addlatexequation/) | Adds an equation object to the worksheet using LaTeX format strings. |
| [AddLaTeXEquation(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const char16_t* latex)](./addlatexequation/) | Adds an equation object to the worksheet using LaTeX format strings. |
| [AddLine(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addline/) | Adds a [LineShape](../lineshape/) to the worksheet. |
| [AddLinkedPicture(int32_t topRow, int32_t leftColumn, int32_t height, int32_t width, const U16String\& sourceFullName)](./addlinkedpicture/) | Add a linked picture. |
| [AddLinkedPicture(int32_t topRow, int32_t leftColumn, int32_t height, int32_t width, const char16_t* sourceFullName)](./addlinkedpicture/) | Add a linked picture. |
| [AddListBox(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addlistbox/) | Adds a [ListBox](../listbox/) to the worksheet. |
| [AddOleObject(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector \<uint8_t\>\& imageData)](./addoleobject/) | Adds an [OleObject](../oleobject/). |
| [AddOleObjectWithLinkedImage(int32_t topRow, int32_t leftColumn, int32_t height, int32_t width, const U16String\& sourceFullName)](./addoleobjectwithlinkedimage/) | Add a linked picture. |
| [AddOleObjectWithLinkedImage(int32_t topRow, int32_t leftColumn, int32_t height, int32_t width, const char16_t* sourceFullName)](./addoleobjectwithlinkedimage/) | Add a linked picture. |
| [AddOval(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addoval/) | Adds a [Oval](../oval/) to the worksheet. |
| [AddPicture(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn, const Vector \<uint8_t\>\& stream)](./addpicture/) | Adds a picture to the collection. |
| [AddPicture(int32_t topRow, int32_t leftColumn, const Vector \<uint8_t\>\& stream, int32_t widthScale, int32_t heightScale)](./addpicture/) | Adds a picture to the collection. |
| [AddPictureInChart(int32_t top, int32_t left, const Vector \<uint8_t\>\& stream, int32_t widthScale, int32_t heightScale)](./addpictureinchart/) | Adds a picture to the chart. |
| [AddRadioButton(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addradiobutton/) | Adds a [RadioButton](../radiobutton/) to the worksheet. |
| [AddRectangle(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addrectangle/) | Adds a [RectangleShape](../rectangleshape/) to the worksheet. |
| [AddScrollBar(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addscrollbar/) | Adds a [ScrollBar](../scrollbar/) to the worksheet. |
| [AddShape(MsoDrawingType type, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addshape/) | Adds a [Shape](../shape/) to the worksheet. |
| [AddShapeInChart(MsoDrawingType type, PlacementType placement, int32_t left, int32_t top, int32_t right, int32_t bottom, const Vector \<uint8_t\>\& imageData)](./addshapeinchart/) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [AddShapeInChart(MsoDrawingType type, PlacementType placement, int32_t left, int32_t top, int32_t right, int32_t bottom)](./addshapeinchart/) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, double top, double right, double bottom)](./addshapeinchartbyscale/) | Add a shape to chart. All unit is percent scale of chart area. |
| [AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, double top, double right, double bottom, const Vector \<uint8_t\>\& imageData)](./addshapeinchartbyscale/) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [AddSignatureLine(int32_t topRow, int32_t leftColumn, const SignatureLine\& signatureLine)](./addsignatureline/) | Adds a Signature [Line](../line/) to the worksheet. |
| [AddSpinner(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addspinner/) | Adds a [Spinner](../spinner/) to the worksheet. |
| [AddSvg(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector \<uint8_t\>\& svgData, const Vector \<uint8_t\>\& compatibleImageData)](./addsvg/) | Adds svg image. |
| [AddTextBox(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addtextbox/) | Adds a text box to the worksheet. |
| [AddTextBoxInChart(int32_t top, int32_t left, int32_t height, int32_t width)](./addtextboxinchart/) | Adds a textbox to the chart. |
| [AddTextEffect(MsoPresetTextEffect effect, const U16String\& text, const U16String\& fontName, int32_t size, bool fontBold, bool fontItalic, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addtexteffect/) | Inserts a WordArt object. |
| [AddTextEffect(MsoPresetTextEffect effect, const char16_t* text, const char16_t* fontName, int32_t size, bool fontBold, bool fontItalic, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addtexteffect/) | Inserts a WordArt object. |
| [AddTextEffectInChart(MsoPresetTextEffect effect, const U16String\& text, const U16String\& fontName, int32_t size, bool fontBold, bool fontItalic, int32_t top, int32_t left, int32_t height, int32_t width)](./addtexteffectinchart/) | Inserts a WordArt object to the chart. |
| [AddTextEffectInChart(MsoPresetTextEffect effect, const char16_t* text, const char16_t* fontName, int32_t size, bool fontBold, bool fontItalic, int32_t top, int32_t left, int32_t height, int32_t width)](./addtexteffectinchart/) | Inserts a WordArt object to the chart. |
| [AddWordArt(PresetWordArtStyle style, const U16String\& text, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addwordart/) | Adds preset WordArt since Excel 2007.s. |
| [AddWordArt(PresetWordArtStyle style, const char16_t* text, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)](./addwordart/) | Adds preset WordArt since Excel 2007.s. |
| [Clear()](./clear/) | Clear all shapes in the worksheet. |
| [CopyCommentsInRange(const ShapeCollection\& shapes, const CellArea\& ca, int32_t destRow, int32_t destColumn)](./copycommentsinrange/) | Copy all comments in the range. |
| [CopyInRange(const ShapeCollection\& sourceShapes, const CellArea\& ca, int32_t destRow, int32_t destColumn, bool isContained)](./copyinrange/) | Copy shapes in the range to destination range. |
| [DeleteInRange(const CellArea\& ca)](./deleteinrange/) | Delete shapes in the range.Comment shapes will not be deleted. |
| [DeleteShape(const Shape\& shape)](./deleteshape/) | Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted. |
| [Get(int32_t index)](./get/) | Gets the [Shape](../shape/) object at the specific index in the list. |
| [Get(const U16String\& name)](./get/) | Gets the [Shape](../shape/) object by the name of the shape. |
| [Get(const char16_t* name)](./get/) | Gets the [Shape](../shape/) object by the name of the shape. |
| [GetCount()](./getcount/) |  |
| [Group(const Vector \<Shape\>\& groupItems)](./group/) | Group the shapes. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ShapeCollection\& src)](./operator_asm/) | operator= |
| [Remove(const Shape\& shape)](./remove/) | Remove the shape. |
| [RemoveAt(int32_t index)](./removeat/) | Remove the shape. |
| [ShapeCollection(ShapeCollection_Impl* impl)](./shapecollection/) | Constructs from an implementation object. |
| [ShapeCollection(const ShapeCollection\& src)](./shapecollection/) | Copy constructor. |
| [Ungroup(const GroupShape\& group)](./ungroup/) | Ungroups the shape items. |
| [UpdateSelectedValue()](./updateselectedvalue/) | Update the selected value by the value of the linked cell or range of the shape. |
| [~ShapeCollection()](./~shapecollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;

//get ShapeCollection
ShapeCollection shapes = workbook.GetWorksheets().Get(0).GetShapes();


//Save the excel file.
workbook.Save("result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
