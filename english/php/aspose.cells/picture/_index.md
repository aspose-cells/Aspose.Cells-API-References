---
title: "Picture Class"
linktitle: "Picture"
articleTitle: "Picture"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents a single picture in a spreadsheet."
type: docs
weight: 4400
url: /php/aspose.cells/picture/
---

## Picture class

Encapsulates the object that represents a single picture in a spreadsheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsPlacedInCell](#isplacedincell) | boolean |  |
| [OriginalHeight](#originalheight) | Number | Gets the original height of the picture. |
| [OriginalWidth](#originalwidth) | Number | Gets the original width of the picture. |
| [BorderLineColor](#borderlinecolor) | Color | Represents the com.aspose.cells.Color of the border line of a picture. |
| [BorderWeight](#borderweight) | Number | Gets or sets the weight of the border line of a picture in units of pt. |
| [Data](#data) | byte[] | Gets the data of the picture. |
| [SourceFullName](#sourcefullname) | String | Gets or sets the path and name of the source file for the linked image. The default value is an empty string. If SourceF |
| [Formula](#formula) | String | Gets and sets the data of the formula. |
| [IsAutoSize](#isautosize) | boolean | True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when |
| [IsLink](#islink) | boolean | Returns true if the picture is linked to a file. |
| [IsDynamicDataExchange](#isdynamicdataexchange) | boolean | Gets or sets whether dynamic data exchange |
| [DisplayAsIcon](#displayasicon) | boolean | True if the specified object is displayed as an icon and the image will not be auto changed. |
| [ImageType](#imagetype) | Number | Gets the image format of the picture. The value of the property is ImageType integer constant. |
| [OriginalHeightCM](#originalheightcm) | Number | Gets the original height of picture, in unit of centimeters. |
| [OriginalWidthCM](#originalwidthcm) | Number | Gets the original width of picture, in unit of centimeters. |
| [OriginalHeightInch](#originalheightinch) | Number | Gets the original height of picture, in unit of inches. |
| [OriginalWidthInch](#originalwidthinch) | Number | Gets the original width of picture, in unit of inches. |
| [SignatureLine](#signatureline) | SignatureLine | Gets and sets the signature line |
| [MacroName](#macroname) | String | Gets and sets the name of macro. |
| [IsEquation](#isequation) | boolean | Indicates whether the shape only contains an equation. |
| [IsSmartArt](#issmartart) | boolean | Indicates whether the shape is a smart art. Only for ooxml file. |
| [ZOrderPosition](#zorderposition) | Number | Returns the position of a shape in the z-order. |
| [Name](#name) | String | Gets and sets the name of the shape. |
| [AlternativeText](#alternativetext) | String | Returns or sets the descriptive (alternative) text string of the Shape object. |
| [Title](#title) | String | Specifies the title (caption) of the current shape object. |
| [LineFormat](#lineformat) | MsoLineFormat | Returns a MsoLineFormat object that contains line formatting properties for the specified shape. NOTE: This member is no |
| [FillFormat](#fillformat) | MsoFillFormat | Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. NOTE: This member is no |
| [Line](#line) | LineFormat | Gets line style |
| [Fill](#fill) | FillFormat | Returns a FillFormat object that contains fill formatting properties for the specified shape. |
| [ShadowEffect](#shadoweffect) | ShadowEffect | Represents a ShadowEffect object that specifies shadow effect for the chart element or shape. |
| [Reflection](#reflection) | ReflectionEffect | Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape. |
| [Glow](#glow) | GlowEffect | Represents a GlowEffect object that specifies glow effect for the chart element or shape. |
| [SoftEdges](#softedges) | Number | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [ThreeDFormat](#threedformat) | ThreeDFormat | Gets and sets 3d format of the shape. |
| [FormatPicture](#formatpicture) | MsoFormatPicture | Gets and sets the options of the picture format. |
| [IsHidden](#ishidden) | boolean | Indicates whether the object is visible. |
| [IsLockAspectRatio](#islockaspectratio) | boolean | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolet |
| [IsAspectRatioLocked](#isaspectratiolocked) | boolean | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. |
| [RotationAngle](#rotationangle) | Number | Gets and sets the rotation of the shape. |
| [Hyperlink](#hyperlink) | Hyperlink | Gets the hyperlink of the shape. |
| [Id](#id) | Number | Gets the identifier of this shape. |
| [Spid](#spid) | String | Specifies an optional string identifier that an application can use to identify the particular shape. |
| [Spt](#spt) | Number | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [Worksheet](#worksheet) | Worksheet | Gets the Worksheet object which contains this shape. |
| [IsGroup](#isgroup) | boolean | Indicates whether this shape is a group shape. |
| [IsInGroup](#isingroup) | boolean | Indicates whether the shape is grouped. |
| [IsWordArt](#iswordart) | boolean | Indicates whether this shape is a word art. Only for the Legacy Shape of xls file. |
| [TextEffect](#texteffect) | TextEffectFormat | Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Sh |
| [IsLocked](#islocked) | boolean | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the wo |
| [IsPrintable](#isprintable) | boolean | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [MsoDrawingType](#msodrawingtype) | Number | Gets drawing type. The value of the property is MsoDrawingType integer constant. |
| [AutoShapeType](#autoshapetype) | Number | Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant. |
| [AnchorType](#anchortype) | Number | Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant. |
| [Placement](#placement) | Number | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an objec |
| [UpperLeftRow](#upperleftrow) | Number | Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored. |
| [UpperDeltaY](#upperdeltay) | Number | Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256. |
| [UpperLeftColumn](#upperleftcolumn) | Number | Represents upper left corner column index. |
| [UpperDeltaX](#upperdeltax) | Number | Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024. |
| [LowerRightRow](#lowerrightrow) | Number | Represents lower right corner row index. |
| [LowerDeltaY](#lowerdeltay) | Number | Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256. |
| [LowerRightColumn](#lowerrightcolumn) | Number | Represents lower right corner column index. |
| [LowerDeltaX](#lowerdeltax) | Number | Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024. |
| [Right](#right) | Number | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [Bottom](#bottom) | Number | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [Width](#width) | Number | Represents the width of shape, in unit of pixels. |
| [WidthInch](#widthinch) | Number | Represents the width of the shape, in unit of inch. |
| [WidthPt](#widthpt) | Number | Represents the width of the shape, in unit of point. |
| [WidthCM](#widthcm) | Number | Represents the width of the shape, in unit of centimeters. |
| [Height](#height) | Number | Represents the height of shape, in unit of pixel. |
| [HeightInch](#heightinch) | Number | Represents the height of the shape, in unit of inches. |
| [HeightPt](#heightpt) | Number | Represents the height of the shape, in unit of points. |
| [HeightCM](#heightcm) | Number | Represents the height of the shape, in unit of centimeters. |
| [Left](#left) | Number | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [LeftInch](#leftinch) | Number | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [LeftCM](#leftcm) | Number | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [Top](#top) | Number | Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents th |
| [TopInch](#topinch) | Number | Represents the vertical offset of shape from its top row, in unit of inches. |
| [TopCM](#topcm) | Number | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [TopToCorner](#toptocorner) | Number | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [LeftToCorner](#lefttocorner) | Number | Gets and sets the horizonal offset of shape from worksheet left border. |
| [X](#x) | Number | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [Y](#y) | Number | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [WidthScale](#widthscale) | Number | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthS |
| [HeightScale](#heightscale) | Number | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the Heigh |
| [TopInShape](#topinshape) | Number | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [LeftInShape](#leftinshape) | Number | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the pa |
| [WidthInShape](#widthinshape) | Number | Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or c |
| [HeightInShape](#heightinshape) | Number | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [Group](#group) | GroupShape | Gets the group shape which contains this shape. |
| [Type](#type) | Number | Gets the auto shape type. The value of the property is AutoShapeType integer constant. |
| [HasLine](#hasline) | boolean | Gets and sets the line border of the shape is visible. |
| [IsFilled](#isfilled) | boolean | Indicates whether the fill format is visible. |
| [IsFlippedHorizontally](#isflippedhorizontally) | boolean | Gets and sets whether shape is horizontally flipped . |
| [IsFlippedVertically](#isflippedvertically) | boolean | Gets and sets whether shape is vertically flipped . |
| [ActualLowerRightRow](#actuallowerrightrow) | Number | Get the actual bottom row. |
| [RelativeToOriginalPictureSize](#relativetooriginalpicturesize) | boolean | Indicates whether shape is relative to original picture size. |
| [LinkedCell](#linkedcell) | String | Gets or sets the worksheet range linked to the control's value. |
| [InputRange](#inputrange) | String | Gets or sets the worksheet range used to fill the specified combo box. |
| [TextShapeType](#textshapetype) | Number | Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant. |
| [TextBody](#textbody) | FontSettingCollection | Gets and sets the setting of the shape's text. |
| [Font](#font) | Font | Represents the font of shape. |
| [TextOptions](#textoptions) | TextOptions | Represents the text options of the shape. |
| [Text](#text) | String | Gets and sets the text of this shape. |
| [IsRichText](#isrichtext) | boolean | Whether or not the text is rich text. |
| [HtmlText](#htmltext) | String | Gets and sets the html string which contains data and some formats in this textbox. |
| [TextVerticalOverflow](#textverticaloverflow) | Number | Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflo |
| [TextHorizontalOverflow](#texthorizontaloverflow) | Number | Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverf |
| [IsTextWrapped](#istextwrapped) | boolean | Gets and sets the text wrapped type of the shape which contains text. |
| [TextOrientationType](#textorientationtype) | Number | Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant. |
| [TextHorizontalAlignment](#texthorizontalalignment) | Number | Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer co |
| [TextVerticalAlignment](#textverticalalignment) | Number | Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer cons |
| [TextDirection](#textdirection) | Number | Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constan |
| [TextBoxOptions](#textboxoptions) | TextBoxOptions |  |
| [ControlData](#controldata) | byte[] | Gets the data of control. |
| [Paths](#paths) | ShapePathCollection | Gets the paths of a custom geometric shape. |
| [Geometry](#geometry) | Geometry | Gets the geometry |
| [CreateId](#createid) | UUID | Gets and sets create id for this shape. |
| [IsDecorative](#isdecorative) | boolean | Indicates whether the object is decorative. |

## Methods

| Name | Description |
| --- | --- |
| [copy](#copy) | Copy the picture. |
| [move](#move) | Moves the picture to a specified location. |
| [placeInCell](#placeincell) | Place this picture in the cell |
| [isSameSetting](#issamesetting) | Returns whether the shape is same. |
| [getLinkedCell](#getlinkedcell) | Gets the range linked to the control's value. |
| [setLinkedCell](#setlinkedcell) | Sets the range linked to the control's value. |
| [getInputRange](#getinputrange) | Gets the range used to fill the control. |
| [setInputRange](#setinputrange) | Sets the range used to fill the control. |
| [updateSelectedValue](#updateselectedvalue) | Update the selected value by the value of the linked cell. |
| [calculateTextSize](#calculatetextsize) | Recalculate the text area |
| [formatCharacters](#formatcharacters) | Formats some characters with the font setting. |
| [characters](#characters) | Returns a Characters object that represents a range of characters within the text.

This method only works on shape with |
| [getCharacters](#getcharacters) | Returns all Characters objects that represents a range of characters within the text .

NOTE: This method is now obsolet |
| [getRichFormattings](#getrichformattings) | Returns all Characters objects that represents a range of characters within the text . |
| [removeActiveXControl](#removeactivexcontrol) | Remove activeX control. |
| [getActualBox](#getactualbox) | Get the actual position and size of the shape (after applying rotation, flip, etc.)

Note:The interface is not fully fun |
| [fitToTextSize](#fittotextsize) |  |
| [getConnectionPoints](#getconnectionpoints) | Get the connection points |
| [toImage](#toimage) | Saves the shape to a file. |
| [getResultOfSmartArt](#getresultofsmartart) | Converting smart art to grouped shapes. |
| [toFrontOrBack](#tofrontorback) | Brings the shape to the front or sends the shape to back. |
| [getLockedProperty](#getlockedproperty) | Gets the value of locked property. |
| [setLockedProperty](#setlockedproperty) | Set the locked property. |
| [addHyperlink](#addhyperlink) | Adds a hyperlink to the shape. |
| [removeHyperlink](#removehyperlink) | Removes the hyperlink of the shape. |
| [moveToRange](#movetorange) | Moves the shape to a specified range. |
| [alignTopRightCorner](#aligntoprightcorner) | Moves the picture to the top-right corner. |

### Picture.IsPlacedInCell property {#isplacedincell}

**Type:** boolean

### Picture.OriginalHeight property {#originalheight}

Gets the original height of the picture.

**Type:** Number

### Picture.OriginalWidth property {#originalwidth}

Gets the original width of the picture.

**Type:** Number

### Picture.BorderLineColor property {#borderlinecolor}

Represents the com.aspose.cells.Color of the border line of a picture.

**Type:** Color

### Picture.BorderWeight property {#borderweight}

Gets or sets the weight of the border line of a picture in units of pt.

**Type:** Number

### Picture.Data property {#data}

Gets the data of the picture.

**Type:** byte[]

### Picture.SourceFullName property {#sourcefullname}

Gets or sets the path and name of the source file for the linked image. The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

**Type:** String

### Picture.Formula property {#formula}

Gets and sets the data of the formula.

**Type:** String

### Picture.IsAutoSize property {#isautosize}

True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

**Type:** boolean

### Picture.IsLink property {#islink}

Returns true if the picture is linked to a file.

**Type:** boolean

### Picture.IsDynamicDataExchange property {#isdynamicdataexchange}

Gets or sets whether dynamic data exchange

**Type:** boolean

### Picture.DisplayAsIcon property {#displayasicon}

True if the specified object is displayed as an icon and the image will not be auto changed.

**Type:** boolean

### Picture.ImageType property {#imagetype}

Gets the image format of the picture. The value of the property is ImageType integer constant.

**Type:** Number

### Picture.OriginalHeightCM property {#originalheightcm}

Gets the original height of picture, in unit of centimeters.

**Type:** Number

### Picture.OriginalWidthCM property {#originalwidthcm}

Gets the original width of picture, in unit of centimeters.

**Type:** Number

### Picture.OriginalHeightInch property {#originalheightinch}

Gets the original height of picture, in unit of inches.

**Type:** Number

### Picture.OriginalWidthInch property {#originalwidthinch}

Gets the original width of picture, in unit of inches.

**Type:** Number

### Picture.SignatureLine property {#signatureline}

Gets and sets the signature line

**Type:** SignatureLine

### Picture.MacroName property {#macroname}

Gets and sets the name of macro.

**Type:** String

### Picture.IsEquation property {#isequation}

Indicates whether the shape only contains an equation.

**Type:** boolean

### Picture.IsSmartArt property {#issmartart}

Indicates whether the shape is a smart art. Only for ooxml file.

**Type:** boolean

### Picture.ZOrderPosition property {#zorderposition}

Returns the position of a shape in the z-order.

**Type:** Number

### Picture.Name property {#name}

Gets and sets the name of the shape.

**Type:** String

### Picture.AlternativeText property {#alternativetext}

Returns or sets the descriptive (alternative) text string of the Shape object.

**Type:** String

### Picture.Title property {#title}

Specifies the title (caption) of the current shape object.

**Type:** String

### Picture.LineFormat property {#lineformat}

Returns a MsoLineFormat object that contains line formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** MsoLineFormat

### Picture.FillFormat property {#fillformat}

Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** MsoFillFormat

### Picture.Line property {#line}

Gets line style

**Type:** LineFormat

### Picture.Fill property {#fill}

Returns a FillFormat object that contains fill formatting properties for the specified shape.

**Type:** FillFormat

### Picture.ShadowEffect property {#shadoweffect}

Represents a ShadowEffect object that specifies shadow effect for the chart element or shape.

**Type:** ShadowEffect

### Picture.Reflection property {#reflection}

Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape.

**Type:** ReflectionEffect

### Picture.Glow property {#glow}

Represents a GlowEffect object that specifies glow effect for the chart element or shape.

**Type:** GlowEffect

### Picture.SoftEdges property {#softedges}

Gets and sets the radius of blur to apply to the edges, in unit of points.

**Type:** Number

### Picture.ThreeDFormat property {#threedformat}

Gets and sets 3d format of the shape.

**Type:** ThreeDFormat

### Picture.FormatPicture property {#formatpicture}

Gets and sets the options of the picture format.

**Type:** MsoFormatPicture

### Picture.IsHidden property {#ishidden}

Indicates whether the object is visible.

**Type:** boolean

### Picture.IsLockAspectRatio property {#islockaspectratio}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### Picture.IsAspectRatioLocked property {#isaspectratiolocked}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects.

**Type:** boolean

### Picture.RotationAngle property {#rotationangle}

Gets and sets the rotation of the shape.

**Type:** Number

### Picture.Hyperlink property {#hyperlink}

Gets the hyperlink of the shape.

**Type:** Hyperlink

### Picture.Id property {#id}

Gets the identifier of this shape.

**Type:** Number

### Picture.Spid property {#spid}

Specifies an optional string identifier that an application can use to identify the particular shape.

**Type:** String

### Picture.Spt property {#spt}

Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

**Type:** Number

### Picture.Worksheet property {#worksheet}

Gets the Worksheet object which contains this shape.

**Type:** Worksheet

### Picture.IsGroup property {#isgroup}

Indicates whether this shape is a group shape.

**Type:** boolean

### Picture.IsInGroup property {#isingroup}

Indicates whether the shape is grouped.

**Type:** boolean

### Picture.IsWordArt property {#iswordart}

Indicates whether this shape is a word art. Only for the Legacy Shape of xls file.

**Type:** boolean

### Picture.TextEffect property {#texteffect}

Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

**Type:** TextEffectFormat

### Picture.IsLocked property {#islocked}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

**Type:** boolean

### Picture.IsPrintable property {#isprintable}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

**Type:** boolean

### Picture.MsoDrawingType property {#msodrawingtype}

Gets drawing type. The value of the property is MsoDrawingType integer constant.

**Type:** Number

### Picture.AutoShapeType property {#autoshapetype}

Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant.

**Type:** Number

### Picture.AnchorType property {#anchortype}

Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant.

**Type:** Number

### Picture.Placement property {#placement}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. The value of the property is PlacementType integer constant.

**Type:** Number

### Picture.UpperLeftRow property {#upperleftrow}

Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

**Type:** Number

### Picture.UpperDeltaY property {#upperdeltay}

Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

**Type:** Number

### Picture.UpperLeftColumn property {#upperleftcolumn}

Represents upper left corner column index.

**Type:** Number

### Picture.UpperDeltaX property {#upperdeltax}

Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

**Type:** Number

### Picture.LowerRightRow property {#lowerrightrow}

Represents lower right corner row index.

**Type:** Number

### Picture.LowerDeltaY property {#lowerdeltay}

Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

**Type:** Number

### Picture.LowerRightColumn property {#lowerrightcolumn}

Represents lower right corner column index.

**Type:** Number

### Picture.LowerDeltaX property {#lowerdeltax}

Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

**Type:** Number

### Picture.Right property {#right}

Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

**Type:** Number

### Picture.Bottom property {#bottom}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

**Type:** Number

### Picture.Width property {#width}

Represents the width of shape, in unit of pixels.

**Type:** Number

### Picture.WidthInch property {#widthinch}

Represents the width of the shape, in unit of inch.

**Type:** Number

### Picture.WidthPt property {#widthpt}

Represents the width of the shape, in unit of point.

**Type:** Number

### Picture.WidthCM property {#widthcm}

Represents the width of the shape, in unit of centimeters.

**Type:** Number

### Picture.Height property {#height}

Represents the height of shape, in unit of pixel.

**Type:** Number

### Picture.HeightInch property {#heightinch}

Represents the height of the shape, in unit of inches.

**Type:** Number

### Picture.HeightPt property {#heightpt}

Represents the height of the shape, in unit of points.

**Type:** Number

### Picture.HeightCM property {#heightcm}

Represents the height of the shape, in unit of centimeters.

**Type:** Number

### Picture.Left property {#left}

Represents the horizontal offset of shape from its left column, in unit of pixels.

**Type:** Number

### Picture.LeftInch property {#leftinch}

Represents the horizontal offset of shape from its left column, in unit of inches.

**Type:** Number

### Picture.LeftCM property {#leftcm}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

**Type:** Number

### Picture.Top property {#top}

Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

**Type:** Number

### Picture.TopInch property {#topinch}

Represents the vertical offset of shape from its top row, in unit of inches.

**Type:** Number

### Picture.TopCM property {#topcm}

Represents the vertical offset of shape from its top row, in unit of centimeters.

**Type:** Number

### Picture.TopToCorner property {#toptocorner}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

**Type:** Number

### Picture.LeftToCorner property {#lefttocorner}

Gets and sets the horizonal offset of shape from worksheet left border.

**Type:** Number

### Picture.X property {#x}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

**Type:** Number

### Picture.Y property {#y}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

**Type:** Number

### Picture.WidthScale property {#widthscale}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

**Type:** Number

### Picture.HeightScale property {#heightscale}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

**Type:** Number

### Picture.TopInShape property {#topinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. Only Applies when this shape in the group or chart.

**Type:** Number

### Picture.LeftInShape property {#leftinshape}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. Only Applies when this shape in the group or chart.

**Type:** Number

### Picture.WidthInShape property {#widthinshape}

Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or chart.

**Type:** Number

### Picture.HeightInShape property {#heightinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. Only Applies when this shape in the group or chart.

**Type:** Number

### Picture.Group property {#group}

Gets the group shape which contains this shape.

**Type:** GroupShape

### Picture.Type property {#type}

Gets the auto shape type. The value of the property is AutoShapeType integer constant.

**Type:** Number

### Picture.HasLine property {#hasline}

Gets and sets the line border of the shape is visible.

**Type:** boolean

### Picture.IsFilled property {#isfilled}

Indicates whether the fill format is visible.

**Type:** boolean

### Picture.IsFlippedHorizontally property {#isflippedhorizontally}

Gets and sets whether shape is horizontally flipped .

**Type:** boolean

### Picture.IsFlippedVertically property {#isflippedvertically}

Gets and sets whether shape is vertically flipped .

**Type:** boolean

### Picture.ActualLowerRightRow property {#actuallowerrightrow}

Get the actual bottom row.

**Type:** Number

### Picture.RelativeToOriginalPictureSize property {#relativetooriginalpicturesize}

Indicates whether shape is relative to original picture size.

**Type:** boolean

### Picture.LinkedCell property {#linkedcell}

Gets or sets the worksheet range linked to the control's value.

**Type:** String

### Picture.InputRange property {#inputrange}

Gets or sets the worksheet range used to fill the specified combo box.

**Type:** String

### Picture.TextShapeType property {#textshapetype}

Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant.

**Type:** Number

### Picture.TextBody property {#textbody}

Gets and sets the setting of the shape's text.

**Type:** FontSettingCollection

### Picture.Font property {#font}

Represents the font of shape.

**Type:** Font

### Picture.TextOptions property {#textoptions}

Represents the text options of the shape.

**Type:** TextOptions

### Picture.Text property {#text}

Gets and sets the text of this shape.

**Type:** String

### Picture.IsRichText property {#isrichtext}

Whether or not the text is rich text.

**Type:** boolean

### Picture.HtmlText property {#htmltext}

Gets and sets the html string which contains data and some formats in this textbox.

**Type:** String

### Picture.TextVerticalOverflow property {#textverticaloverflow}

Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

**Type:** Number

### Picture.TextHorizontalOverflow property {#texthorizontaloverflow}

Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

**Type:** Number

### Picture.IsTextWrapped property {#istextwrapped}

Gets and sets the text wrapped type of the shape which contains text.

**Type:** boolean

### Picture.TextOrientationType property {#textorientationtype}

Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant.

**Type:** Number

### Picture.TextHorizontalAlignment property {#texthorizontalalignment}

Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### Picture.TextVerticalAlignment property {#textverticalalignment}

Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### Picture.TextDirection property {#textdirection}

Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constant.

**Type:** Number

### Picture.TextBoxOptions property {#textboxoptions}

**Type:** TextBoxOptions

### Picture.ControlData property {#controldata}

Gets the data of control.

**Type:** byte[]

### Picture.Paths property {#paths}

Gets the paths of a custom geometric shape.

**Type:** ShapePathCollection

### Picture.Geometry property {#geometry}

Gets the geometry

**Type:** Geometry

### Picture.CreateId property {#createid}

Gets and sets create id for this shape.

**Type:** UUID

### Picture.IsDecorative property {#isdecorative}

Indicates whether the object is decorative.

**Type:** boolean

### copy(source, options) {#copy}

Copy the picture.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Picture | The source picture. |
| options | CopyOptions | The copy options. |

### move(topRow, leftColumn) {#move}

Moves the picture to a specified location.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |

### placeInCell() {#placeincell}

Place this picture in the cell

### isSameSetting(obj) {#issamesetting}

Returns whether the shape is same.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### getLinkedCell(isR1C1, isLocal) {#getlinkedcell}

Gets the range linked to the control's value.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The range linked to the control's value.

### setLinkedCell(formula, isR1C1, isLocal) {#setlinkedcell}

Sets the range linked to the control's value.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The range linked to the control's value. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### getInputRange(isR1C1, isLocal) {#getinputrange}

Gets the range used to fill the control.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The range used to fill the control.

### setInputRange(formula, isR1C1, isLocal) {#setinputrange}

Sets the range used to fill the control.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The range used to fill the control. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### updateSelectedValue() {#updateselectedvalue}

Update the selected value by the value of the linked cell.

### calculateTextSize() {#calculatetextsize}

Recalculate the text area

**Returns:** Text's Size in an array(width and height).

### formatCharacters(startIndex, length, font, flag) {#formatcharacters}

Formats some characters with the font setting.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The start index. |
| length | Number | The length. |
| font | Font | The font setting. |
| flag | StyleFlag | The flag of the font setting. |

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the text.

This method only works on shape with title.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** Characters object.

### getCharacters() {#getcharacters}

Returns all Characters objects that represents a range of characters within the text .

NOTE: This method is now obsolete. Instead, please use Shape.GetRichFormattings() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** All Characters objects

### getRichFormattings() {#getrichformattings}

Returns all Characters objects that represents a range of characters within the text .

**Returns:** All Characters objects

### removeActiveXControl() {#removeactivexcontrol}

Remove activeX control.

### getActualBox() {#getactualbox}

Get the actual position and size of the shape (after applying rotation, flip, etc.)

Note:The interface is not fully functional, especially the location information is not correct.It is recommended not to use this interface until the function is complete.

**Returns:** Return the position and size in the order of x, y, w, h

### fitToTextSize() {#fittotextsize}

### getConnectionPoints() {#getconnectionpoints}

Get the connection points

**Returns:** [X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### toImage(imageFile, options) {#toimage}

Saves the shape to a file.

### getResultOfSmartArt() {#getresultofsmartart}

Converting smart art to grouped shapes.

### toFrontOrBack(orders) {#tofrontorback}

Brings the shape to the front or sends the shape to back.

| Parameter | Type | Description |
| --- | --- | --- |
| orders | Number | If it's less than zero, sets the shape to back. If it's greater than zero, brings the shape to front. |

### getLockedProperty(type) {#getlockedproperty}

Gets the value of locked property.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A ShapeLockType value. The type of the shape locked property. |

**Returns:** Returns the value of locked property.

### setLockedProperty(type, value) {#setlockedproperty}

Set the locked property.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A ShapeLockType value. The locked type. |
| value | boolean | The value of the property. |

### addHyperlink(address) {#addhyperlink}

Adds a hyperlink to the shape.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |

**Returns:** Return the new hyperlink object.

### removeHyperlink() {#removehyperlink}

Removes the hyperlink of the shape.

### moveToRange(topRow, leftColumn, bottomRow, rightColumn) {#movetorange}

Moves the shape to a specified range.

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow |  | Upper left row index. |
| upperLeftColumn |  | Upper left column index. |
| lowerRightRow |  | Lower right row index |
| lowerRightColumn |  | Lower right column index |

### alignTopRightCorner(topRow, rightColumn) {#aligntoprightcorner}

Moves the picture to the top-right corner.

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Number | the row index. |
| rightColumn | Number | the column index. |
