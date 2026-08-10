---
title: "OleObject Class"
linktitle: "OleObject"
articleTitle: "OleObject"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents an OleObject in a worksheet."
type: docs
weight: 4050
url: /php/aspose.cells/oleobject/
---

## OleObject class

Represents an OleObject in a worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsAutoSize](#isautosize) | boolean | True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when |
| [IsLink](#islink) | boolean | Returns true if the OleObject links to the file. |
| [DisplayAsIcon](#displayasicon) | boolean | True if the specified object is displayed as an icon and the image will not be auto changed. |
| [ImageData](#imagedata) | byte[] | Represents image of ole object as byte array. |
| [ObjectData](#objectdata) | byte[] | Represents embedded ole object data as byte array. |
| [FullObjectBin](#fullobjectbin) | byte[] | Gets the full embedded ole object binary data in the template file. |
| [ImageSourceFullName](#imagesourcefullname) | String | Gets or sets the path and name of the source file for the linked image. The default value is an empty string. If SourceF |
| [ProgID](#progid) | String | Gets or sets the ProgID of the OLE object. |
| [FileFormatType](#fileformattype) | Number | Gets and sets the file type of the embedded ole object data The value of the property is FileFormatType integer constant |
| [ObjectSourceFullName](#objectsourcefullname) | String | Returns the source full name of the source file for the linked OLE object. Only supports setting the source full name wh |
| [Label](#label) | String | Gets and sets the display label of the linked ole object. |
| [AutoUpdate](#autoupdate) | boolean | Specifies whether the link to the OleObject is automatically updated or not. |
| [AutoLoad](#autoload) | boolean | Specifies whether the host application for the embedded object shall be called to load the object data automatically whe |
| [ClassIdentifier](#classidentifier) | byte[] | Gets and sets the class identifier of the embedded object. It means which application opens the embedded file. |
| [ImageType](#imagetype) | Number | Gets the image format of the ole object. The value of the property is ImageType integer constant. |
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
| [setEmbeddedObject](#setembeddedobject) | Sets embedded object data. |
| [setNativeSourceFullName](#setnativesourcefullname) | Sets the ole native source full file name with path. |
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
| [isSameSetting](#issamesetting) | Returns whether the shape is same. |
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

### OleObject.IsAutoSize property {#isautosize}

True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

**Type:** boolean

### OleObject.IsLink property {#islink}

Returns true if the OleObject links to the file.

**Type:** boolean

### OleObject.DisplayAsIcon property {#displayasicon}

True if the specified object is displayed as an icon and the image will not be auto changed.

**Type:** boolean

### OleObject.ImageData property {#imagedata}

Represents image of ole object as byte array.

**Type:** byte[]

### OleObject.ObjectData property {#objectdata}

Represents embedded ole object data as byte array.

**Type:** byte[]

### OleObject.FullObjectBin property {#fullobjectbin}

Gets the full embedded ole object binary data in the template file.

**Type:** byte[]

### OleObject.ImageSourceFullName property {#imagesourcefullname}

Gets or sets the path and name of the source file for the linked image. The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

**Type:** String

### OleObject.ProgID property {#progid}

Gets or sets the ProgID of the OLE object.

**Type:** String

### OleObject.FileFormatType property {#fileformattype}

Gets and sets the file type of the embedded ole object data The value of the property is FileFormatType integer constant.

**Type:** Number

### OleObject.ObjectSourceFullName property {#objectsourcefullname}

Returns the source full name of the source file for the linked OLE object. Only supports setting the source full name when the file type is OleFileType.Unknown. Such as wav file ,avi file..etc..

**Type:** String

### OleObject.Label property {#label}

Gets and sets the display label of the linked ole object.

**Type:** String

### OleObject.AutoUpdate property {#autoupdate}

Specifies whether the link to the OleObject is automatically updated or not.

**Type:** boolean

### OleObject.AutoLoad property {#autoload}

Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened.

**Type:** boolean

### OleObject.ClassIdentifier property {#classidentifier}

Gets and sets the class identifier of the embedded object. It means which application opens the embedded file.

**Type:** byte[]

### OleObject.ImageType property {#imagetype}

Gets the image format of the ole object. The value of the property is ImageType integer constant.

**Type:** Number

### OleObject.MacroName property {#macroname}

Gets and sets the name of macro.

**Type:** String

### OleObject.IsEquation property {#isequation}

Indicates whether the shape only contains an equation.

**Type:** boolean

### OleObject.IsSmartArt property {#issmartart}

Indicates whether the shape is a smart art. Only for ooxml file.

**Type:** boolean

### OleObject.ZOrderPosition property {#zorderposition}

Returns the position of a shape in the z-order.

**Type:** Number

### OleObject.Name property {#name}

Gets and sets the name of the shape.

**Type:** String

### OleObject.AlternativeText property {#alternativetext}

Returns or sets the descriptive (alternative) text string of the Shape object.

**Type:** String

### OleObject.Title property {#title}

Specifies the title (caption) of the current shape object.

**Type:** String

### OleObject.LineFormat property {#lineformat}

Returns a MsoLineFormat object that contains line formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** MsoLineFormat

### OleObject.FillFormat property {#fillformat}

Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** MsoFillFormat

### OleObject.Line property {#line}

Gets line style

**Type:** LineFormat

### OleObject.Fill property {#fill}

Returns a FillFormat object that contains fill formatting properties for the specified shape.

**Type:** FillFormat

### OleObject.ShadowEffect property {#shadoweffect}

Represents a ShadowEffect object that specifies shadow effect for the chart element or shape.

**Type:** ShadowEffect

### OleObject.Reflection property {#reflection}

Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape.

**Type:** ReflectionEffect

### OleObject.Glow property {#glow}

Represents a GlowEffect object that specifies glow effect for the chart element or shape.

**Type:** GlowEffect

### OleObject.SoftEdges property {#softedges}

Gets and sets the radius of blur to apply to the edges, in unit of points.

**Type:** Number

### OleObject.ThreeDFormat property {#threedformat}

Gets and sets 3d format of the shape.

**Type:** ThreeDFormat

### OleObject.FormatPicture property {#formatpicture}

Gets and sets the options of the picture format.

**Type:** MsoFormatPicture

### OleObject.IsHidden property {#ishidden}

Indicates whether the object is visible.

**Type:** boolean

### OleObject.IsLockAspectRatio property {#islockaspectratio}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### OleObject.IsAspectRatioLocked property {#isaspectratiolocked}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects.

**Type:** boolean

### OleObject.RotationAngle property {#rotationangle}

Gets and sets the rotation of the shape.

**Type:** Number

### OleObject.Hyperlink property {#hyperlink}

Gets the hyperlink of the shape.

**Type:** Hyperlink

### OleObject.Id property {#id}

Gets the identifier of this shape.

**Type:** Number

### OleObject.Spid property {#spid}

Specifies an optional string identifier that an application can use to identify the particular shape.

**Type:** String

### OleObject.Spt property {#spt}

Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

**Type:** Number

### OleObject.Worksheet property {#worksheet}

Gets the Worksheet object which contains this shape.

**Type:** Worksheet

### OleObject.IsGroup property {#isgroup}

Indicates whether this shape is a group shape.

**Type:** boolean

### OleObject.IsInGroup property {#isingroup}

Indicates whether the shape is grouped.

**Type:** boolean

### OleObject.IsWordArt property {#iswordart}

Indicates whether this shape is a word art. Only for the Legacy Shape of xls file.

**Type:** boolean

### OleObject.TextEffect property {#texteffect}

Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

**Type:** TextEffectFormat

### OleObject.IsLocked property {#islocked}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

**Type:** boolean

### OleObject.IsPrintable property {#isprintable}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

**Type:** boolean

### OleObject.MsoDrawingType property {#msodrawingtype}

Gets drawing type. The value of the property is MsoDrawingType integer constant.

**Type:** Number

### OleObject.AutoShapeType property {#autoshapetype}

Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant.

**Type:** Number

### OleObject.AnchorType property {#anchortype}

Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant.

**Type:** Number

### OleObject.Placement property {#placement}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. The value of the property is PlacementType integer constant.

**Type:** Number

### OleObject.UpperLeftRow property {#upperleftrow}

Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

**Type:** Number

### OleObject.UpperDeltaY property {#upperdeltay}

Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

**Type:** Number

### OleObject.UpperLeftColumn property {#upperleftcolumn}

Represents upper left corner column index.

**Type:** Number

### OleObject.UpperDeltaX property {#upperdeltax}

Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

**Type:** Number

### OleObject.LowerRightRow property {#lowerrightrow}

Represents lower right corner row index.

**Type:** Number

### OleObject.LowerDeltaY property {#lowerdeltay}

Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

**Type:** Number

### OleObject.LowerRightColumn property {#lowerrightcolumn}

Represents lower right corner column index.

**Type:** Number

### OleObject.LowerDeltaX property {#lowerdeltax}

Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

**Type:** Number

### OleObject.Right property {#right}

Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

**Type:** Number

### OleObject.Bottom property {#bottom}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

**Type:** Number

### OleObject.Width property {#width}

Represents the width of shape, in unit of pixels.

**Type:** Number

### OleObject.WidthInch property {#widthinch}

Represents the width of the shape, in unit of inch.

**Type:** Number

### OleObject.WidthPt property {#widthpt}

Represents the width of the shape, in unit of point.

**Type:** Number

### OleObject.WidthCM property {#widthcm}

Represents the width of the shape, in unit of centimeters.

**Type:** Number

### OleObject.Height property {#height}

Represents the height of shape, in unit of pixel.

**Type:** Number

### OleObject.HeightInch property {#heightinch}

Represents the height of the shape, in unit of inches.

**Type:** Number

### OleObject.HeightPt property {#heightpt}

Represents the height of the shape, in unit of points.

**Type:** Number

### OleObject.HeightCM property {#heightcm}

Represents the height of the shape, in unit of centimeters.

**Type:** Number

### OleObject.Left property {#left}

Represents the horizontal offset of shape from its left column, in unit of pixels.

**Type:** Number

### OleObject.LeftInch property {#leftinch}

Represents the horizontal offset of shape from its left column, in unit of inches.

**Type:** Number

### OleObject.LeftCM property {#leftcm}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

**Type:** Number

### OleObject.Top property {#top}

Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

**Type:** Number

### OleObject.TopInch property {#topinch}

Represents the vertical offset of shape from its top row, in unit of inches.

**Type:** Number

### OleObject.TopCM property {#topcm}

Represents the vertical offset of shape from its top row, in unit of centimeters.

**Type:** Number

### OleObject.TopToCorner property {#toptocorner}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

**Type:** Number

### OleObject.LeftToCorner property {#lefttocorner}

Gets and sets the horizonal offset of shape from worksheet left border.

**Type:** Number

### OleObject.X property {#x}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

**Type:** Number

### OleObject.Y property {#y}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

**Type:** Number

### OleObject.WidthScale property {#widthscale}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

**Type:** Number

### OleObject.HeightScale property {#heightscale}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

**Type:** Number

### OleObject.TopInShape property {#topinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. Only Applies when this shape in the group or chart.

**Type:** Number

### OleObject.LeftInShape property {#leftinshape}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. Only Applies when this shape in the group or chart.

**Type:** Number

### OleObject.WidthInShape property {#widthinshape}

Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or chart.

**Type:** Number

### OleObject.HeightInShape property {#heightinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. Only Applies when this shape in the group or chart.

**Type:** Number

### OleObject.Group property {#group}

Gets the group shape which contains this shape.

**Type:** GroupShape

### OleObject.Type property {#type}

Gets the auto shape type. The value of the property is AutoShapeType integer constant.

**Type:** Number

### OleObject.HasLine property {#hasline}

Gets and sets the line border of the shape is visible.

**Type:** boolean

### OleObject.IsFilled property {#isfilled}

Indicates whether the fill format is visible.

**Type:** boolean

### OleObject.IsFlippedHorizontally property {#isflippedhorizontally}

Gets and sets whether shape is horizontally flipped .

**Type:** boolean

### OleObject.IsFlippedVertically property {#isflippedvertically}

Gets and sets whether shape is vertically flipped .

**Type:** boolean

### OleObject.ActualLowerRightRow property {#actuallowerrightrow}

Get the actual bottom row.

**Type:** Number

### OleObject.RelativeToOriginalPictureSize property {#relativetooriginalpicturesize}

Indicates whether shape is relative to original picture size.

**Type:** boolean

### OleObject.LinkedCell property {#linkedcell}

Gets or sets the worksheet range linked to the control's value.

**Type:** String

### OleObject.InputRange property {#inputrange}

Gets or sets the worksheet range used to fill the specified combo box.

**Type:** String

### OleObject.TextShapeType property {#textshapetype}

Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant.

**Type:** Number

### OleObject.TextBody property {#textbody}

Gets and sets the setting of the shape's text.

**Type:** FontSettingCollection

### OleObject.Font property {#font}

Represents the font of shape.

**Type:** Font

### OleObject.TextOptions property {#textoptions}

Represents the text options of the shape.

**Type:** TextOptions

### OleObject.Text property {#text}

Gets and sets the text of this shape.

**Type:** String

### OleObject.IsRichText property {#isrichtext}

Whether or not the text is rich text.

**Type:** boolean

### OleObject.HtmlText property {#htmltext}

Gets and sets the html string which contains data and some formats in this textbox.

**Type:** String

### OleObject.TextVerticalOverflow property {#textverticaloverflow}

Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

**Type:** Number

### OleObject.TextHorizontalOverflow property {#texthorizontaloverflow}

Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

**Type:** Number

### OleObject.IsTextWrapped property {#istextwrapped}

Gets and sets the text wrapped type of the shape which contains text.

**Type:** boolean

### OleObject.TextOrientationType property {#textorientationtype}

Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant.

**Type:** Number

### OleObject.TextHorizontalAlignment property {#texthorizontalalignment}

Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### OleObject.TextVerticalAlignment property {#textverticalalignment}

Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### OleObject.TextDirection property {#textdirection}

Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constant.

**Type:** Number

### OleObject.TextBoxOptions property {#textboxoptions}

**Type:** TextBoxOptions

### OleObject.ControlData property {#controldata}

Gets the data of control.

**Type:** byte[]

### OleObject.Paths property {#paths}

Gets the paths of a custom geometric shape.

**Type:** ShapePathCollection

### OleObject.Geometry property {#geometry}

Gets the geometry

**Type:** Geometry

### OleObject.CreateId property {#createid}

Gets and sets create id for this shape.

**Type:** UUID

### OleObject.IsDecorative property {#isdecorative}

Indicates whether the object is decorative.

**Type:** boolean

### setEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label) (1 of 2) {#setembeddedobject}

Sets embedded object data.

| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | byte[] | The embedded object data. |
| sourceFileName | String | The file name. |
| displayAsIcon | boolean | Indicates whether diplaying object as an icon. If true, the orginal image data will be covered by icon. |
| label | String | The icon label. Only works when displayAsIcon as true. |

---

### setEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon) (2 of 2) {#setembeddedobject-1}

Sets embedded object data.

As Aspose can update embedd all file icons, so it's better that you can add correct icon with updateIcon as false.

| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | byte[] | The embedded object data. |
| sourceFileName | String | The file name. |
| displayAsIcon | boolean | Indicates whether diplaying object as an icon. If true, the orginal image data will be covered by icon. |
| label | String | The icon label. Only works when displayAsIcon as true. |
| updateIcon | boolean | Indicates whether automatically updating icon. |

### setNativeSourceFullName(sourceFullName) {#setnativesourcefullname}

Sets the ole native source full file name with path.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceFullName | String | the ole native source full file name |

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

### isSameSetting(obj) {#issamesetting}

Returns whether the shape is same.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

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
