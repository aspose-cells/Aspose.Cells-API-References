﻿---
title: Aspose::Cells::Drawing::Shape class
linktitle: Shape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape class. Represents the msodrawing object in C++.'
type: docs
weight: 5100
url: /cpp/aspose.cells.drawing/shape/
---
## Shape class


Represents the msodrawing object.

```cpp
class Shape
```

## Methods

| Method | Description |
| --- | --- |
| [AddHyperlink(const U16String\& address)](./addhyperlink/) | Adds a hyperlink to the shape. |
| [AddHyperlink(const char16_t* address)](./addhyperlink/) | Adds a hyperlink to the shape. |
| [AlignTopRightCorner(int32_t topRow, int32_t rightColumn)](./aligntoprightcorner/) | Moves the picture to the top-right corner. |
| [CalculateTextSize()](./calculatetextsize/) | Recalculate the text area. |
| [Characters(int32_t startIndex, int32_t length)](./characters/) | Returns a Characters object that represents a range of characters within the text. |
| [FormatCharacters(int32_t startIndex, int32_t length, const Aspose::Cells::Font\& font, const StyleFlag\& flag)](./formatcharacters/) | Formats some characters with the font setting. |
| [GetActiveXControl()](./getactivexcontrol/) | Gets the ActiveX control. |
| [GetActualBox()](./getactualbox/) | Get the actual position and size of the shape (after applying rotation, flip, etc.) |
| [GetActualLowerRightRow()](./getactuallowerrightrow/) | Get the actual bottom row. |
| [GetAlternativeText()](./getalternativetext/) | Returns or sets the descriptive (alternative) text string of the [Shape](./) object. |
| [GetAnchorType()](./getanchortype/) | Gets and set the shape anchor placeholder. |
| [GetAutoShapeType()](./getautoshapetype/) | Gets and sets the auto shape type. |
| [GetBottom()](./getbottom/) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [GetControlData()](./getcontroldata/) | Gets the data of control. |
| [GetFill()](./getfill/) | Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape. |
| [GetFont()](./getfont/) | Represents the font of shape. |
| [GetFormatPicture()](./getformatpicture/) | Gets and sets the options of the picture format. |
| [GetGeometry()](./getgeometry/) | Gets the geometry. |
| [GetGlow()](./getglow/) | Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape. |
| [GetGroup()](./getgroup/) | Gets the group shape which contains this shape. |
| [GetHasLine()](./gethasline/) | Gets and sets the line border of the shape is visible. |
| [GetHeight()](./getheight/) | Represents the height of shape, in unit of pixel. |
| [GetHeightCM()](./getheightcm/) | Represents the height of the shape, in unit of centimeters. |
| [GetHeightInch()](./getheightinch/) | Represents the height of the shape, in unit of inches. |
| [GetHeightInShape()](./getheightinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [GetHeightPt()](./getheightpt/) | Represents the height of the shape, in unit of points. |
| [GetHeightScale()](./getheightscale/) | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;. |
| [GetHtmlText()](./gethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
| [GetHyperlink()](./gethyperlink/) | Gets the hyperlink of the shape. |
| [GetId()](./getid/) | Gets the identifier of this shape. |
| [GetInputRange()](./getinputrange/) | Gets or sets the worksheet range used to fill the specified combo box. |
| [GetInputRange(bool isR1C1, bool isLocal)](./getinputrange/) | Gets the range used to fill the control. |
| [GetLeft()](./getleft/) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [GetLeftCM()](./getleftcm/) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [GetLeftInch()](./getleftinch/) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [GetLeftInShape()](./getleftinshape/) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [GetLeftToCorner()](./getlefttocorner/) | Gets and sets the horizonal offset of shape from worksheet left border. |
| [GetLine()](./getline/) | Gets line style. |
| [GetLinkedCell()](./getlinkedcell/) | Gets or sets the worksheet range linked to the control's value. |
| [GetLinkedCell(bool isR1C1, bool isLocal)](./getlinkedcell/) | Gets the range linked to the control's value. |
| [GetLockedProperty(ShapeLockType type)](./getlockedproperty/) | Gets the value of locked property. |
| [GetLowerDeltaX()](./getlowerdeltax/) | Gets or sets the shape's horizontal offset from its lower right corner column. |
| [GetLowerDeltaY()](./getlowerdeltay/) | Gets or sets the shape's vertical offset from its lower right corner row. |
| [GetLowerRightColumn()](./getlowerrightcolumn/) | Represents lower right corner column index. |
| [GetLowerRightRow()](./getlowerrightrow/) | Represents lower right corner row index. |
| [GetMacroName()](./getmacroname/) | Gets and sets the name of macro. |
| [GetMsoDrawingType()](./getmsodrawingtype/) | Gets mso drawing type. |
| [GetName()](./getname/) | Gets and sets the name of the shape. |
| [GetPaths()](./getpaths/) | Gets the paths of a custom geometric shape. |
| [GetPlacement()](./getplacement/) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [GetReflection()](./getreflection/) | Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape. |
| [GetRelativeToOriginalPictureSize()](./getrelativetooriginalpicturesize/) | Indicates whether shape is relative to original picture size. |
| [GetResultOfSmartArt()](./getresultofsmartart/) | Converting smart art to grouped shapes. |
| [GetRichFormattings()](./getrichformattings/) | Returns all Characters objects that represents a range of characters within the text . |
| [GetRight()](./getright/) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [GetRotationAngle()](./getrotationangle/) | Gets and sets the rotation of the shape. |
| [GetShadowEffect()](./getshadoweffect/) | Represents a [Drawing.ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [GetSoftEdges()](./getsoftedges/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [GetSpid()](./getspid/) | Specifies an optional string that an application can use to Identify the particular shape. |
| [GetSpt()](./getspt/) | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [GetText()](./gettext/) | Represents the string in this [TextBox](../textbox/) object. |
| [GetTextBody()](./gettextbody/) | Gets and sets the setting of the shape's text. |
| [GetTextDirection()](./gettextdirection/) | Gets/Sets the direction of the text flow for this object. |
| [GetTextEffect()](./gettexteffect/) | Returns a [TextEffectFormat](../texteffectformat/) object that contains text-effect formatting properties for the specified shape. Applies to [Shape](./) objects that represent WordArt. |
| [GetTextHorizontalAlignment()](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the shape. |
| [GetTextHorizontalOverflow()](./gettexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the shape which contains text. |
| [GetTextOptions()](./gettextoptions/) | Represents the text options of the shape. |
| [GetTextOrientationType()](./gettextorientationtype/) | Gets and sets the text orientation type of the shape. |
| [GetTextShapeType()](./gettextshapetype/) | Gets and sets the preset text shape type. |
| [GetTextVerticalAlignment()](./gettextverticalalignment/) | Gets and sets the text vertical alignment type of the shape. |
| [GetTextVerticalOverflow()](./gettextverticaloverflow/) | Gets and sets the text vertical overflow type of the shape which contains text. |
| [GetThreeDFormat()](./getthreedformat/) | Gets and sets 3d format of the shape. |
| [GetTitle()](./gettitle/) | Specifies the title (caption) of the current shape object. |
| [GetTop()](./gettop/) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [GetTopCM()](./gettopcm/) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [GetTopInch()](./gettopinch/) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [GetTopInShape()](./gettopinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [GetTopToCorner()](./gettoptocorner/) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [GetType()](./gettype/) | Gets the auto shape type. |
| [GetUpperDeltaX()](./getupperdeltax/) | Gets or sets the shape's horizontal offset from its upper left corner column. |
| [GetUpperDeltaY()](./getupperdeltay/) | Gets or sets the shape's vertical offset from its upper left corner row. |
| [GetUpperLeftColumn()](./getupperleftcolumn/) | Represents upper left corner column index. |
| [GetUpperLeftRow()](./getupperleftrow/) | Represents upper left corner row index. |
| [GetWidth()](./getwidth/) | Represents the width of shape, in unit of pixels. |
| [GetWidthCM()](./getwidthcm/) | Represents the width of the shape, in unit of centimeters. |
| [GetWidthInch()](./getwidthinch/) | Represents the width of the shape, in unit of inch. |
| [GetWidthInShape()](./getwidthinshape/) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [GetWidthPt()](./getwidthpt/) | Represents the width of the shape, in unit of point. |
| [GetWidthScale()](./getwidthscale/) | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;. |
| [GetWorksheet()](./getworksheet/) | Gets the [Worksheet](../../aspose.cells/worksheet/) object which contains this shape. |
| [GetX()](./getx/) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [GetY()](./gety/) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [GetZOrderPosition()](./getzorderposition/) | Returns the position of a shape in the z-order. |
| [IsEquation()](./isequation/) | Indicates whether the shape only contains an equation. |
| [IsFilled()](./isfilled/) | Indicates whether the fill format is visible. |
| [IsFlippedHorizontally()](./isflippedhorizontally/) | Gets and sets whether shape is horizontally flipped . |
| [IsFlippedVertically()](./isflippedvertically/) | Gets and sets whether shape is vertically flipped . |
| [IsGroup()](./isgroup/) | Indicates whether the shape is a group. |
| [IsHidden()](./ishidden/) | Indicates whether the object is visible. |
| [IsInGroup()](./isingroup/) | Indicates whether the shape is grouped. |
| [IsLockAspectRatio()](./islockaspectratio/) | True means that don't allow changes in aspect ratio. |
| [IsLocked()](./islocked/) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsPrintable()](./isprintable/) | True if the object is printable. |
| [IsRichText()](./isrichtext/) | Whether or not the text is rich text. |
| [IsSmartArt()](./issmartart/) | Indicates whether the shape is smart art. |
| [IsTextWrapped()](./istextwrapped/) | Gets and sets the text wrapped type of the shape which contains text. |
| [IsWordArt()](./iswordart/) | Indicates whether this shape is a word art. |
| [MoveToRange(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t lowerRightRow, int32_t lowerRightColumn)](./movetorange/) | Moves the shape to a specified range. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Shape\& src)](./operator_asm/) | operator= |
| [RemoveActiveXControl()](./removeactivexcontrol/) | Remove activeX control. |
| [RemoveHyperlink()](./removehyperlink/) | Remove the hyperlink of the shape. |
| [SetAlternativeText(const U16String\& value)](./setalternativetext/) | Returns or sets the descriptive (alternative) text string of the [Shape](./) object. |
| [SetAlternativeText(const char16_t* value)](./setalternativetext/) | Returns or sets the descriptive (alternative) text string of the [Shape](./) object. |
| [SetAnchorType(ShapeAnchorType value)](./setanchortype/) | Gets and set the shape anchor placeholder. |
| [SetAutoShapeType(AutoShapeType value)](./setautoshapetype/) | Gets and sets the auto shape type. |
| [SetBottom(int32_t value)](./setbottom/) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [SetFont(const Aspose::Cells::Font\& value)](./setfont/) | Represents the font of shape. |
| [SetHasLine(bool value)](./sethasline/) | Gets and sets the line border of the shape is visible. |
| [SetHeight(int32_t value)](./setheight/) | Represents the height of shape, in unit of pixel. |
| [SetHeightCM(double value)](./setheightcm/) | Represents the height of the shape, in unit of centimeters. |
| [SetHeightInch(double value)](./setheightinch/) | Represents the height of the shape, in unit of inches. |
| [SetHeightInShape(int32_t value)](./setheightinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [SetHeightPt(double value)](./setheightpt/) | Represents the height of the shape, in unit of points. |
| [SetHeightScale(int32_t value)](./setheightscale/) | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;. |
| [SetHtmlText(const U16String\& value)](./sethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
| [SetHtmlText(const char16_t* value)](./sethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
| [SetInputRange(const U16String\& value)](./setinputrange/) | Gets or sets the worksheet range used to fill the specified combo box. |
| [SetInputRange(const char16_t* value)](./setinputrange/) | Gets or sets the worksheet range used to fill the specified combo box. |
| [SetInputRange(const U16String\& formula, bool isR1C1, bool isLocal)](./setinputrange/) | Sets the range used to fill the control. |
| [SetInputRange(const char16_t* formula, bool isR1C1, bool isLocal)](./setinputrange/) | Sets the range used to fill the control. |
| [SetIsFilled(bool value)](./setisfilled/) | Indicates whether the fill format is visible. |
| [SetIsFlippedHorizontally(bool value)](./setisflippedhorizontally/) | Gets and sets whether shape is horizontally flipped . |
| [SetIsFlippedVertically(bool value)](./setisflippedvertically/) | Gets and sets whether shape is vertically flipped . |
| [SetIsHidden(bool value)](./setishidden/) | Indicates whether the object is visible. |
| [SetIsLockAspectRatio(bool value)](./setislockaspectratio/) | True means that don't allow changes in aspect ratio. |
| [SetIsLocked(bool value)](./setislocked/) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [SetIsPrintable(bool value)](./setisprintable/) | True if the object is printable. |
| [SetIsTextWrapped(bool value)](./setistextwrapped/) | Gets and sets the text wrapped type of the shape which contains text. |
| [SetLeft(int32_t value)](./setleft/) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [SetLeftCM(double value)](./setleftcm/) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [SetLeftInch(double value)](./setleftinch/) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [SetLeftInShape(int32_t value)](./setleftinshape/) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [SetLeftToCorner(int32_t value)](./setlefttocorner/) | Gets and sets the horizonal offset of shape from worksheet left border. |
| [SetLinkedCell(const U16String\& value)](./setlinkedcell/) | Gets or sets the worksheet range linked to the control's value. |
| [SetLinkedCell(const char16_t* value)](./setlinkedcell/) | Gets or sets the worksheet range linked to the control's value. |
| [SetLinkedCell(const U16String\& formula, bool isR1C1, bool isLocal)](./setlinkedcell/) | Sets the range linked to the control's value. |
| [SetLinkedCell(const char16_t* formula, bool isR1C1, bool isLocal)](./setlinkedcell/) | Sets the range linked to the control's value. |
| [SetLockedProperty(ShapeLockType type, bool value)](./setlockedproperty/) | Set the locked property. |
| [SetLowerDeltaX(int32_t value)](./setlowerdeltax/) | Gets or sets the shape's horizontal offset from its lower right corner column. |
| [SetLowerDeltaY(int32_t value)](./setlowerdeltay/) | Gets or sets the shape's vertical offset from its lower right corner row. |
| [SetLowerRightColumn(int32_t value)](./setlowerrightcolumn/) | Represents lower right corner column index. |
| [SetLowerRightRow(int32_t value)](./setlowerrightrow/) | Represents lower right corner row index. |
| [SetMacroName(const U16String\& value)](./setmacroname/) | Gets and sets the name of macro. |
| [SetMacroName(const char16_t* value)](./setmacroname/) | Gets and sets the name of macro. |
| [SetName(const U16String\& value)](./setname/) | Gets and sets the name of the shape. |
| [SetName(const char16_t* value)](./setname/) | Gets and sets the name of the shape. |
| [SetPlacement(PlacementType value)](./setplacement/) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [SetRelativeToOriginalPictureSize(bool value)](./setrelativetooriginalpicturesize/) | Indicates whether shape is relative to original picture size. |
| [SetRight(int32_t value)](./setright/) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [SetRotationAngle(double value)](./setrotationangle/) | Gets and sets the rotation of the shape. |
| [SetSoftEdges(double value)](./setsoftedges/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [SetText(const U16String\& value)](./settext/) | Represents the string in this [TextBox](../textbox/) object. |
| [SetText(const char16_t* value)](./settext/) | Represents the string in this [TextBox](../textbox/) object. |
| [SetTextDirection(TextDirectionType value)](./settextdirection/) | Gets/Sets the direction of the text flow for this object. |
| [SetTextHorizontalAlignment(TextAlignmentType value)](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the shape. |
| [SetTextHorizontalOverflow(TextOverflowType value)](./settexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the shape which contains text. |
| [SetTextOptions(const TextOptions\& value)](./settextoptions/) | Represents the text options of the shape. |
| [SetTextOrientationType(TextOrientationType value)](./settextorientationtype/) | Gets and sets the text orientation type of the shape. |
| [SetTextShapeType(AutoShapeType value)](./settextshapetype/) | Gets and sets the preset text shape type. |
| [SetTextVerticalAlignment(TextAlignmentType value)](./settextverticalalignment/) | Gets and sets the text vertical alignment type of the shape. |
| [SetTextVerticalOverflow(TextOverflowType value)](./settextverticaloverflow/) | Gets and sets the text vertical overflow type of the shape which contains text. |
| [SetTitle(const U16String\& value)](./settitle/) | Specifies the title (caption) of the current shape object. |
| [SetTitle(const char16_t* value)](./settitle/) | Specifies the title (caption) of the current shape object. |
| [SetTop(int32_t value)](./settop/) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [SetTopCM(double value)](./settopcm/) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [SetTopInch(double value)](./settopinch/) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [SetTopInShape(int32_t value)](./settopinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [SetTopToCorner(int32_t value)](./settoptocorner/) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [SetUpperDeltaX(int32_t value)](./setupperdeltax/) | Gets or sets the shape's horizontal offset from its upper left corner column. |
| [SetUpperDeltaY(int32_t value)](./setupperdeltay/) | Gets or sets the shape's vertical offset from its upper left corner row. |
| [SetUpperLeftColumn(int32_t value)](./setupperleftcolumn/) | Represents upper left corner column index. |
| [SetUpperLeftRow(int32_t value)](./setupperleftrow/) | Represents upper left corner row index. |
| [SetWidth(int32_t value)](./setwidth/) | Represents the width of shape, in unit of pixels. |
| [SetWidthCM(double value)](./setwidthcm/) | Represents the width of the shape, in unit of centimeters. |
| [SetWidthInch(double value)](./setwidthinch/) | Represents the width of the shape, in unit of inch. |
| [SetWidthInShape(int32_t value)](./setwidthinshape/) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [SetWidthPt(double value)](./setwidthpt/) | Represents the width of the shape, in unit of point. |
| [SetWidthScale(int32_t value)](./setwidthscale/) | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;. |
| [SetX(int32_t value)](./setx/) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [SetY(int32_t value)](./sety/) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [SetZOrderPosition(int32_t value)](./setzorderposition/) | Returns the position of a shape in the z-order. |
| [Shape(Shape_Impl* impl)](./shape/) | Constructs from an implementation object. |
| [Shape(const Shape\& src)](./shape/) | Copy constructor. |
| [ToFrontOrBack(int32_t orders)](./tofrontorback/) | Brings the shape to the front or sends the shape to back. |
| [ToImage(const Vector \<uint8_t\>\& stream, Aspose::Cells::Drawing::ImageType imageType)](./toimage/) | Creates the shape image and saves it to a stream in the specified format. |
| [ToImage(const U16String\& imageFile, const ImageOrPrintOptions\& options)](./toimage/) | Saves the shape to a file. |
| [ToImage(const char16_t* imageFile, const ImageOrPrintOptions\& options)](./toimage/) | Saves the shape to a file. |
| [ToImage(const ImageOrPrintOptions\& options)](./toimage/) | Saves the shape to a stream. |
| [UpdateSelectedValue()](./updateselectedvalue/) | Update the selected value by the value of the linked cell. |
| [~Shape()](./~shape/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Initialize a new workbook.
Workbook book;

//Add a shape.(e.g rectangle)
Shape shape = book.GetWorksheets().Get(0).GetShapes().AddRectangle(2, 0, 2, 0, 130, 130);


//Save the excel file.
book.Save(u"exmaple.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
