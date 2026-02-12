---
title: Aspose::Cells::Drawing::Picture class
linktitle: Picture
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture class. Encapsulates the object that represents a single picture in a spreadsheet in C++.'
type: docs
weight: 4400
url: /cpp/aspose.cells.drawing/picture/
---
## Picture class


Encapsulates the object that represents a single picture in a spreadsheet.

```cpp
class Picture : public Aspose::Cells::Drawing::Shape
```

## Methods

| Method | Description |
| --- | --- |
| [AddHyperlink(const U16String\& address)](../shape/addhyperlink/) | Adds a hyperlink to the shape. |
| [AddHyperlink(const char16_t* address)](../shape/addhyperlink/) | Adds a hyperlink to the shape. |
| [AlignTopRightCorner(int32_t topRow, int32_t rightColumn)](../shape/aligntoprightcorner/) | Moves the picture to the top-right corner. |
| [CalculateTextSize()](../shape/calculatetextsize/) | Recalculate the text area. |
| [Characters(int32_t startIndex, int32_t length)](../shape/characters/) | Returns a Characters object that represents a range of characters within the text. |
| [Copy(const Aspose::Cells::Drawing::Picture\& source, const CopyOptions\& options)](./copy/) | Copy the picture. |
| [FitToTextSize()](../shape/fittotextsize/) | Recalculate a text area suitable for displaying all text content. |
| [FormatCharacters(int32_t startIndex, int32_t length, const Aspose::Cells::Font\& font, const StyleFlag\& flag)](../shape/formatcharacters/) | Formats some characters with the font setting. |
| [GetActiveXControl()](../shape/getactivexcontrol/) | Gets the ActiveX control. |
| [GetActualBox()](../shape/getactualbox/) | Get the actual position and size of the shape (after applying rotation, flip, etc.) |
| [GetActualLowerRightRow()](../shape/getactuallowerrightrow/) | Get the actual bottom row. |
| [GetAlternativeText()](../shape/getalternativetext/) | Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object. |
| [GetAnchorType()](../shape/getanchortype/) | Gets and set the type of the shape anchor placeholder. |
| [GetAutoShapeType()](../shape/getautoshapetype/) | Gets and sets the auto shape type. |
| [GetBorderLineColor()](./getborderlinecolor/) | Represents the [Color](../../aspose.cells/color/) of the border line of a picture. |
| [GetBorderWeight()](./getborderweight/) | Gets or sets the weight of the border line of a picture in units of pt. |
| [GetBottom()](../shape/getbottom/) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [GetConnectionPoints()](../shape/getconnectionpoints/) | Get the connection points. |
| [GetControlData()](../shape/getcontroldata/) | Gets the data of control. |
| [GetCreateId(UUID\& uuid)](../shape/getcreateid/) | Gets and sets create id for this shape. |
| [GetData()](./getdata/) | Gets the data of the picture. |
| [GetDisplayAsIcon()](./getdisplayasicon/) | True if the specified object is displayed as an icon and the image will not be auto changed. |
| [GetFill()](../shape/getfill/) | Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape. |
| [GetFont()](../shape/getfont/) | Represents the font of shape. |
| [GetFormatPicture()](../shape/getformatpicture/) | Gets and sets the options of the picture format. |
| [GetFormula()](./getformula/) | Gets and sets the data of the formula. |
| [GetGeometry()](../shape/getgeometry/) | Gets the geometry. |
| [GetGlow()](../shape/getglow/) | Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape. |
| [GetGroup()](../shape/getgroup/) | Gets the group shape which contains this shape. |
| [GetHasLine()](../shape/gethasline/) | Gets and sets the line border of the shape is visible. |
| [GetHeight()](../shape/getheight/) | Represents the height of shape, in unit of pixel. |
| [GetHeightCM()](../shape/getheightcm/) | Represents the height of the shape, in unit of centimeters. |
| [GetHeightInch()](../shape/getheightinch/) | Represents the height of the shape, in unit of inches. |
| [GetHeightInShape()](../shape/getheightinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [GetHeightPt()](../shape/getheightpt/) | Represents the height of the shape, in unit of points. |
| [GetHeightScale()](../shape/getheightscale/) | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;. |
| [GetHtmlText()](../shape/gethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
| [GetHyperlink()](../shape/gethyperlink/) | Gets the hyperlink of the shape. |
| [GetId()](../shape/getid/) | Gets the identifier of this shape. |
| [GetImageType()](./getimagetype/) | Gets the image format of the picture. |
| [GetInputRange()](../shape/getinputrange/) | Gets or sets the worksheet range used to fill the specified combo box. |
| [GetInputRange(bool isR1C1, bool isLocal)](../shape/getinputrange/) | Gets the range used to fill the control. |
| [GetLeft()](../shape/getleft/) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [GetLeftCM()](../shape/getleftcm/) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [GetLeftInch()](../shape/getleftinch/) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [GetLeftInShape()](../shape/getleftinshape/) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [GetLeftToCorner()](../shape/getlefttocorner/) | Gets and sets the horizonal offset of shape from worksheet left border. |
| [GetLine()](../shape/getline/) | Gets line style. |
| [GetLinkedCell()](../shape/getlinkedcell/) | Gets or sets the worksheet range linked to the control's value. |
| [GetLinkedCell(bool isR1C1, bool isLocal)](../shape/getlinkedcell/) | Gets the range linked to the control's value. |
| [GetLockedProperty(ShapeLockType type)](../shape/getlockedproperty/) | Gets the value of locked property. |
| [GetLowerDeltaX()](../shape/getlowerdeltax/) | Gets or sets the shape's horizontal offset from its lower right corner column. |
| [GetLowerDeltaY()](../shape/getlowerdeltay/) | Gets or sets the shape's vertical offset from its lower right corner row. |
| [GetLowerRightColumn()](../shape/getlowerrightcolumn/) | Represents lower right corner column index. |
| [GetLowerRightRow()](../shape/getlowerrightrow/) | Represents lower right corner row index. |
| [GetMacroName()](../shape/getmacroname/) | Gets and sets the name of macro. |
| [GetMsoDrawingType()](../shape/getmsodrawingtype/) | Gets drawing type. |
| [GetName()](../shape/getname/) | Gets and sets the name of the shape. |
| [GetOriginalHeight()](./getoriginalheight/) | Gets the original height of the picture. |
| [GetOriginalHeightCM()](./getoriginalheightcm/) | Gets the original height of picture, in unit of centimeters. |
| [GetOriginalHeightInch()](./getoriginalheightinch/) | Gets the original height of picture, in unit of inches. |
| [GetOriginalWidth()](./getoriginalwidth/) | Gets the original width of the picture. |
| [GetOriginalWidthCM()](./getoriginalwidthcm/) | Gets the original width of picture, in unit of centimeters. |
| [GetOriginalWidthInch()](./getoriginalwidthinch/) | Gets the original width of picture, in unit of inches. |
| [GetPaths()](../shape/getpaths/) | Gets the paths of a custom geometric shape. |
| [GetPlacement()](../shape/getplacement/) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [GetReflection()](../shape/getreflection/) | Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape. |
| [GetRelativeToOriginalPictureSize()](../shape/getrelativetooriginalpicturesize/) | Indicates whether shape is relative to original picture size. |
| [GetResultOfSmartArt()](../shape/getresultofsmartart/) | Converting smart art to grouped shapes. |
| [GetRichFormattings()](../shape/getrichformattings/) | Returns all Characters objects that represents a range of characters within the text . |
| [GetRight()](../shape/getright/) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [GetRotationAngle()](../shape/getrotationangle/) | Gets and sets the rotation of the shape. |
| [GetShadowEffect()](../shape/getshadoweffect/) | Represents a [Drawing.ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [GetSignatureLine()](./getsignatureline/) | Gets and sets the signature line. |
| [GetSoftEdges()](../shape/getsoftedges/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [GetSourceFullName()](./getsourcefullname/) | Gets or sets the path and name of the source file for the linked image. |
| [GetSpid()](../shape/getspid/) | Specifies an optional string identifier that an application can use to identify the particular shape. |
| [GetSpt()](../shape/getspt/) | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [GetText()](../shape/gettext/) | Gets and sets the text of this shape. |
| [GetTextBody()](../shape/gettextbody/) | Gets and sets the setting of the shape's text. |
| [GetTextBoxOptions()](../shape/gettextboxoptions/) | Gets the text information in the shape. |
| [GetTextDirection()](../shape/gettextdirection/) | Gets/Sets the direction of the text flow for this object. |
| [GetTextEffect()](../shape/gettexteffect/) | Returns a [TextEffectFormat](../texteffectformat/) object that contains text-effect formatting properties for the specified shape. Applies to [Shape](../shape/) objects that represent WordArt. |
| [GetTextHorizontalAlignment()](../shape/gettexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the shape. |
| [GetTextHorizontalOverflow()](../shape/gettexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the shape which contains text. |
| [GetTextOptions()](../shape/gettextoptions/) | Represents the text options of the shape. |
| [GetTextOrientationType()](../shape/gettextorientationtype/) | Gets and sets the text orientation type of the shape. |
| [GetTextShapeType()](../shape/gettextshapetype/) | Gets and sets the preset text shape type. |
| [GetTextVerticalAlignment()](../shape/gettextverticalalignment/) | Gets and sets the text vertical alignment type of the shape. |
| [GetTextVerticalOverflow()](../shape/gettextverticaloverflow/) | Gets and sets the text vertical overflow type of the shape which contains text. |
| [GetThreeDFormat()](../shape/getthreedformat/) | Gets and sets 3d format of the shape. |
| [GetTitle()](../shape/gettitle/) | Specifies the title (caption) of the current shape object. |
| [GetTop()](../shape/gettop/) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [GetTopCM()](../shape/gettopcm/) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [GetTopInch()](../shape/gettopinch/) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [GetTopInShape()](../shape/gettopinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [GetTopToCorner()](../shape/gettoptocorner/) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [GetType()](../shape/gettype/) | Gets the auto shape type. |
| [GetUpperDeltaX()](../shape/getupperdeltax/) | Gets or sets the shape's horizontal offset from its upper left corner column. |
| [GetUpperDeltaY()](../shape/getupperdeltay/) | Gets or sets the shape's vertical offset from its upper left corner row. |
| [GetUpperLeftColumn()](../shape/getupperleftcolumn/) | Represents upper left corner column index. |
| [GetUpperLeftRow()](../shape/getupperleftrow/) | Represents the top row index. |
| [GetWidth()](../shape/getwidth/) | Represents the width of shape, in unit of pixels. |
| [GetWidthCM()](../shape/getwidthcm/) | Represents the width of the shape, in unit of centimeters. |
| [GetWidthInch()](../shape/getwidthinch/) | Represents the width of the shape, in unit of inch. |
| [GetWidthInShape()](../shape/getwidthinshape/) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [GetWidthPt()](../shape/getwidthpt/) | Represents the width of the shape, in unit of point. |
| [GetWidthScale()](../shape/getwidthscale/) | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;. |
| [GetWorksheet()](../shape/getworksheet/) | Gets the [Worksheet](../../aspose.cells/worksheet/) object which contains this shape. |
| [GetX()](../shape/getx/) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [GetY()](../shape/gety/) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [GetZOrderPosition()](../shape/getzorderposition/) | Returns the position of a shape in the z-order. |
| [IsAspectRatioLocked()](../shape/isaspectratiolocked/) | True means that aspect ratio of the shape is locked. |
| [IsAutoSize()](./isautosize/) | True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated. |
| [IsDecorative()](../shape/isdecorative/) | Indicates whether the object is decorative. |
| [IsDynamicDataExchange()](./isdynamicdataexchange/) | Gets or sets whether dynamic data exchange. |
| [IsEquation()](../shape/isequation/) | Indicates whether the shape only contains an equation. |
| [IsFilled()](../shape/isfilled/) | Indicates whether the fill format is visible. |
| [IsFlippedHorizontally()](../shape/isflippedhorizontally/) | Gets and sets whether shape is horizontally flipped . |
| [IsFlippedVertically()](../shape/isflippedvertically/) | Gets and sets whether shape is vertically flipped . |
| [IsGroup()](../shape/isgroup/) | Indicates whether this shape is a group shape. |
| [IsHidden()](../shape/ishidden/) | Indicates whether the object is visible. |
| [IsInGroup()](../shape/isingroup/) | Indicates whether the shape is grouped. |
| [IsLink()](./islink/) | Returns true if the picture is linked to a file. |
| [IsLockAspectRatio()](../shape/islockaspectratio/) |  **(Deprecated)** True means that aspect ratio of the shape is locked. |
| [IsLocked()](../shape/islocked/) | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsPlacedInCell()](./isplacedincell/) | Indicates whether to place the image in cell or over cells. |
| [IsPrintable()](../shape/isprintable/) | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [IsRichText()](../shape/isrichtext/) | Whether or not the text is rich text. |
| [IsSameSetting(const Aspose::Cells::Object\& obj)](./issamesetting/) | Returns whether the shape is same. |
| [IsSmartArt()](../shape/issmartart/) | Indicates whether the shape is a smart art. |
| [IsTextWrapped()](../shape/istextwrapped/) | Gets and sets the text wrapped type of the shape which contains text. |
| [IsWordArt()](../shape/iswordart/) | Indicates whether this shape is a word art. |
| [Move(int32_t topRow, int32_t leftColumn)](./move/) | Moves the picture to a specified location. |
| [MoveToRange(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn)](../shape/movetorange/) | Moves the shape to a specified range. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Aspose::Cells::Drawing::Picture\& src)](./operator_asm/) | operator= |
| [operator=(const Shape\& src)](../shape/operator_asm/) | operator= |
| [Picture(Picture_Impl* impl)](./picture/) | Constructs from an implementation object. |
| [Picture(const Aspose::Cells::Drawing::Picture\& src)](./picture/) | Copy constructor. |
| [Picture(const Shape\& src)](./picture/) | Constructs from a parent object. |
| [PlaceInCell()](./placeincell/) |  **(Deprecated)** Place this picture in the cell. |
| [RemoveActiveXControl()](../shape/removeactivexcontrol/) | Remove activeX control. |
| [RemoveHyperlink()](../shape/removehyperlink/) | Removes the hyperlink of the shape. |
| [SetAlternativeText(const U16String\& value)](../shape/setalternativetext/) | Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object. |
| [SetAlternativeText(const char16_t* value)](../shape/setalternativetext/) | Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object. |
| [SetAnchorType(ShapeAnchorType value)](../shape/setanchortype/) | Gets and set the type of the shape anchor placeholder. |
| [SetAutoShapeType(AutoShapeType value)](../shape/setautoshapetype/) | Gets and sets the auto shape type. |
| [SetBorderLineColor(const Aspose::Cells::Color\& value)](./setborderlinecolor/) | Represents the [Color](../../aspose.cells/color/) of the border line of a picture. |
| [SetBorderWeight(double value)](./setborderweight/) | Gets or sets the weight of the border line of a picture in units of pt. |
| [SetBottom(int32_t value)](../shape/setbottom/) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [SetCreateId(const UUID\& value)](../shape/setcreateid/) | Gets and sets create id for this shape. |
| [SetData(const Vector \<uint8_t\>\& value)](./setdata/) | Gets the data of the picture. |
| [SetDisplayAsIcon(bool value)](./setdisplayasicon/) | True if the specified object is displayed as an icon and the image will not be auto changed. |
| [SetFont(const Aspose::Cells::Font\& value)](../shape/setfont/) | Represents the font of shape. |
| [SetFormula(const U16String\& value)](./setformula/) | Gets and sets the data of the formula. |
| [SetFormula(const char16_t* value)](./setformula/) | Gets and sets the data of the formula. |
| [SetHasLine(bool value)](../shape/sethasline/) | Gets and sets the line border of the shape is visible. |
| [SetHeight(int32_t value)](../shape/setheight/) | Represents the height of shape, in unit of pixel. |
| [SetHeightCM(double value)](../shape/setheightcm/) | Represents the height of the shape, in unit of centimeters. |
| [SetHeightInch(double value)](../shape/setheightinch/) | Represents the height of the shape, in unit of inches. |
| [SetHeightInShape(int32_t value)](../shape/setheightinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [SetHeightPt(double value)](../shape/setheightpt/) | Represents the height of the shape, in unit of points. |
| [SetHeightScale(int32_t value)](../shape/setheightscale/) | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;. |
| [SetHtmlText(const U16String\& value)](../shape/sethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
| [SetHtmlText(const char16_t* value)](../shape/sethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
| [SetInputRange(const U16String\& value)](../shape/setinputrange/) | Gets or sets the worksheet range used to fill the specified combo box. |
| [SetInputRange(const char16_t* value)](../shape/setinputrange/) | Gets or sets the worksheet range used to fill the specified combo box. |
| [SetInputRange(const U16String\& formula, bool isR1C1, bool isLocal)](../shape/setinputrange/) | Sets the range used to fill the control. |
| [SetInputRange(const char16_t* formula, bool isR1C1, bool isLocal)](../shape/setinputrange/) | Sets the range used to fill the control. |
| [SetIsAspectRatioLocked(bool value)](../shape/setisaspectratiolocked/) | True means that aspect ratio of the shape is locked. |
| [SetIsAutoSize(bool value)](./setisautosize/) | True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated. |
| [SetIsDecorative(bool value)](../shape/setisdecorative/) | Indicates whether the object is decorative. |
| [SetIsDynamicDataExchange(bool value)](./setisdynamicdataexchange/) | Gets or sets whether dynamic data exchange. |
| [SetIsFilled(bool value)](../shape/setisfilled/) | Indicates whether the fill format is visible. |
| [SetIsFlippedHorizontally(bool value)](../shape/setisflippedhorizontally/) | Gets and sets whether shape is horizontally flipped . |
| [SetIsFlippedVertically(bool value)](../shape/setisflippedvertically/) | Gets and sets whether shape is vertically flipped . |
| [SetIsHidden(bool value)](../shape/setishidden/) | Indicates whether the object is visible. |
| [SetIsLink(bool value)](./setislink/) | Returns true if the picture is linked to a file. |
| [SetIsLockAspectRatio(bool value)](../shape/setislockaspectratio/) |  **(Deprecated)** True means that aspect ratio of the shape is locked. |
| [SetIsLocked(bool value)](../shape/setislocked/) | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [SetIsPlacedInCell(bool value)](./setisplacedincell/) | Indicates whether to place the image in cell or over cells. |
| [SetIsPrintable(bool value)](../shape/setisprintable/) | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [SetIsTextWrapped(bool value)](../shape/setistextwrapped/) | Gets and sets the text wrapped type of the shape which contains text. |
| [SetLeft(int32_t value)](../shape/setleft/) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [SetLeftCM(double value)](../shape/setleftcm/) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [SetLeftInch(double value)](../shape/setleftinch/) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [SetLeftInShape(int32_t value)](../shape/setleftinshape/) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [SetLeftToCorner(int32_t value)](../shape/setlefttocorner/) | Gets and sets the horizonal offset of shape from worksheet left border. |
| [SetLinkedCell(const U16String\& value)](../shape/setlinkedcell/) | Gets or sets the worksheet range linked to the control's value. |
| [SetLinkedCell(const char16_t* value)](../shape/setlinkedcell/) | Gets or sets the worksheet range linked to the control's value. |
| [SetLinkedCell(const U16String\& formula, bool isR1C1, bool isLocal)](../shape/setlinkedcell/) | Sets the range linked to the control's value. |
| [SetLinkedCell(const char16_t* formula, bool isR1C1, bool isLocal)](../shape/setlinkedcell/) | Sets the range linked to the control's value. |
| [SetLockedProperty(ShapeLockType type, bool value)](../shape/setlockedproperty/) | Set the locked property. |
| [SetLowerDeltaX(int32_t value)](../shape/setlowerdeltax/) | Gets or sets the shape's horizontal offset from its lower right corner column. |
| [SetLowerDeltaY(int32_t value)](../shape/setlowerdeltay/) | Gets or sets the shape's vertical offset from its lower right corner row. |
| [SetLowerRightColumn(int32_t value)](../shape/setlowerrightcolumn/) | Represents lower right corner column index. |
| [SetLowerRightRow(int32_t value)](../shape/setlowerrightrow/) | Represents lower right corner row index. |
| [SetMacroName(const U16String\& value)](../shape/setmacroname/) | Gets and sets the name of macro. |
| [SetMacroName(const char16_t* value)](../shape/setmacroname/) | Gets and sets the name of macro. |
| [SetName(const U16String\& value)](../shape/setname/) | Gets and sets the name of the shape. |
| [SetName(const char16_t* value)](../shape/setname/) | Gets and sets the name of the shape. |
| [SetPlacement(PlacementType value)](../shape/setplacement/) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [SetRelativeToOriginalPictureSize(bool value)](../shape/setrelativetooriginalpicturesize/) | Indicates whether shape is relative to original picture size. |
| [SetRight(int32_t value)](../shape/setright/) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [SetRotationAngle(double value)](../shape/setrotationangle/) | Gets and sets the rotation of the shape. |
| [SetSignatureLine(const SignatureLine\& value)](./setsignatureline/) | Gets and sets the signature line. |
| [SetSoftEdges(double value)](../shape/setsoftedges/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [SetSourceFullName(const U16String\& value)](./setsourcefullname/) | Gets or sets the path and name of the source file for the linked image. |
| [SetSourceFullName(const char16_t* value)](./setsourcefullname/) | Gets or sets the path and name of the source file for the linked image. |
| [SetText(const U16String\& value)](../shape/settext/) | Gets and sets the text of this shape. |
| [SetText(const char16_t* value)](../shape/settext/) | Gets and sets the text of this shape. |
| [SetTextDirection(TextDirectionType value)](../shape/settextdirection/) | Gets/Sets the direction of the text flow for this object. |
| [SetTextHorizontalAlignment(TextAlignmentType value)](../shape/settexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the shape. |
| [SetTextHorizontalOverflow(TextOverflowType value)](../shape/settexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the shape which contains text. |
| [SetTextOptions(const TextOptions\& value)](../shape/settextoptions/) | Represents the text options of the shape. |
| [SetTextOrientationType(TextOrientationType value)](../shape/settextorientationtype/) | Gets and sets the text orientation type of the shape. |
| [SetTextShapeType(AutoShapeType value)](../shape/settextshapetype/) | Gets and sets the preset text shape type. |
| [SetTextVerticalAlignment(TextAlignmentType value)](../shape/settextverticalalignment/) | Gets and sets the text vertical alignment type of the shape. |
| [SetTextVerticalOverflow(TextOverflowType value)](../shape/settextverticaloverflow/) | Gets and sets the text vertical overflow type of the shape which contains text. |
| [SetTitle(const U16String\& value)](../shape/settitle/) | Specifies the title (caption) of the current shape object. |
| [SetTitle(const char16_t* value)](../shape/settitle/) | Specifies the title (caption) of the current shape object. |
| [SetTop(int32_t value)](../shape/settop/) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [SetTopCM(double value)](../shape/settopcm/) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [SetTopInch(double value)](../shape/settopinch/) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [SetTopInShape(int32_t value)](../shape/settopinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [SetTopToCorner(int32_t value)](../shape/settoptocorner/) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [SetUpperDeltaX(int32_t value)](../shape/setupperdeltax/) | Gets or sets the shape's horizontal offset from its upper left corner column. |
| [SetUpperDeltaY(int32_t value)](../shape/setupperdeltay/) | Gets or sets the shape's vertical offset from its upper left corner row. |
| [SetUpperLeftColumn(int32_t value)](../shape/setupperleftcolumn/) | Represents upper left corner column index. |
| [SetUpperLeftRow(int32_t value)](../shape/setupperleftrow/) | Represents the top row index. |
| [SetWidth(int32_t value)](../shape/setwidth/) | Represents the width of shape, in unit of pixels. |
| [SetWidthCM(double value)](../shape/setwidthcm/) | Represents the width of the shape, in unit of centimeters. |
| [SetWidthInch(double value)](../shape/setwidthinch/) | Represents the width of the shape, in unit of inch. |
| [SetWidthInShape(int32_t value)](../shape/setwidthinshape/) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [SetWidthPt(double value)](../shape/setwidthpt/) | Represents the width of the shape, in unit of point. |
| [SetWidthScale(int32_t value)](../shape/setwidthscale/) | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;. |
| [SetX(int32_t value)](../shape/setx/) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [SetY(int32_t value)](../shape/sety/) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [SetZOrderPosition(int32_t value)](../shape/setzorderposition/) | Returns the position of a shape in the z-order. |
| [Shape(Shape_Impl* impl)](../shape/shape/) | Constructs from an implementation object. |
| [Shape(const Shape\& src)](../shape/shape/) | Copy constructor. |
| [ToFrontOrBack(int32_t orders)](../shape/tofrontorback/) | Brings the shape to the front or sends the shape to back. |
| [ToImage(Aspose::Cells::Drawing::ImageType imageType)](../shape/toimage/) | Creates the shape image and saves it to a stream in the specified format. |
| [ToImage(const U16String\& imageFile, const ImageOrPrintOptions\& options)](../shape/toimage/) | Saves the shape to a file. |
| [ToImage(const char16_t* imageFile, const ImageOrPrintOptions\& options)](../shape/toimage/) | Saves the shape to a file. |
| [ToImage(const ImageOrPrintOptions\& options)](../shape/toimage/) | Saves the shape to a stream. |
| [UpdateSelectedValue()](../shape/updateselectedvalue/) | Update the selected value by the value of the linked cell. |
| [~Picture()](./~picture/) | Destructor. |
| [~Shape()](../shape/~shape/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Adding a new worksheet to the Workbook object
int sheetIndex = workbook.GetWorksheets().Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Adding a picture at the location of a cell whose row and column indices
//are 5 in the worksheet. It is "F6" cell
worksheet.GetPictures().Add(5, 5, u"image.gif");
//Saving the Excel file
workbook.Save(u"book1.xls", SaveFormat::Excel97To2003);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Shape](../shape/)
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
