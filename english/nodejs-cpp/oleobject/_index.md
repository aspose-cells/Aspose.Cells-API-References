---
title: OleObject
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents an OleObject in a worksheet.
type: docs
url: /nodejs-cpp/oleobject/
---

## OleObject class

Represents an OleObject in a worksheet.

```javascript
class OleObject extends Shape;
```


### Example
```javascript
const fs = require("fs");
const { Workbook } = require("aspose.cells.node");

//Instantiate a new Workbook.
var workbook = new Workbook();
//Get the first worksheet. 
var sheet = workbook.worksheets.get(0);

//Obtain the picture into the array of bytes from a stream.
var imgBuf = new Uint8Array(fs.readFileSync("input/example.png"));
//Add an Ole object into the worksheet with the bytes
sheet.oleObjects.add(14, 3, 200, 220, imgBuf);
//Set embedded ole object data from a stream.
var fileBuf = new Uint8Array(fs.readFileSync("input/Book1.xls"));
sheet.oleObjects.get(0).objectData = fileBuf;
//Save the excel file
workbook.save("output/DrawingOleObject.xls");
```
## Constructors

| Constructor | Description |
| --- | --- |
| [constructor(Shape)](#constructor-shape-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isAutoSize](#isAutoSize--)| boolean | True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated. |
| [isLink](#isLink--)| boolean | Returns true if the OleObject links to the file. |
| [displayAsIcon](#displayAsIcon--)| boolean | True if the specified object is displayed as an icon and the image will not be auto changed. |
| [imageData](#imageData--)| Uint8Array | Represents image of ole object as byte array. |
| [objectData](#objectData--)| Uint8Array | Represents embedded ole object data as byte array. |
| [fullObjectBin](#fullObjectBin--)| Uint8Array | Readonly. Gets the full embedded ole object binary data in the template file. |
| [imageSourceFullName](#imageSourceFullName--)| string | Gets or sets the path and name of the source file for the linked image. |
| [progID](#progID--)| string | Gets or sets the ProgID of the OLE object. |
| [fileFormatType](#fileFormatType--)| FileFormatType | Gets and sets the file type of the embedded ole object data |
| [objectSourceFullName](#objectSourceFullName--)| string | Returns the source full name of the source file for the linked OLE object. |
| [label](#label--)| string | Gets and sets the display label of the linked ole object. |
| [autoUpdate](#autoUpdate--)| boolean | Specifies whether the link to the OleObject is automatically updated or not. |
| [autoLoad](#autoLoad--)| boolean | Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened. |
| [classIdentifier](#classIdentifier--)| Uint8Array | Gets and sets the class identifier of the embedded object. It means which application opens the embedded file. |
| [imageType](#imageType--)| ImageType | Readonly. Gets the image format of the ole object. |
| [macroName](#macroName--)| string | Gets and sets the name of macro. |
| [isEquation](#isEquation--)| boolean | Readonly. Indicates whether the shape only contains an equation. |
| [isSmartArt](#isSmartArt--)| boolean | Readonly. Indicates whether the shape is a smart art. |
| [zOrderPosition](#zOrderPosition--)| number | Returns the position of a shape in the z-order. |
| [name](#name--)| string | Gets and sets the name of the shape. |
| [alternativeText](#alternativeText--)| string | Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object. |
| [title](#title--)| string | Specifies the title (caption) of the current shape object. |
| [line](#line--)| LineFormat | Readonly. Gets line style |
| [fill](#fill--)| FillFormat | Readonly. Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape. |
| [shadowEffect](#shadowEffect--)| ShadowEffect | Readonly. Represents a [Drawing.ShadowEffect](../drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [reflection](#reflection--)| ReflectionEffect | Readonly. Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape. |
| [glow](#glow--)| GlowEffect | Readonly. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape. |
| [softEdges](#softEdges--)| number | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [threeDFormat](#threeDFormat--)| ThreeDFormat | Readonly. Gets and sets 3d format of the shape. |
| [formatPicture](#formatPicture--)| MsoFormatPicture | Readonly. Gets and sets the options of the picture format. |
| [isHidden](#isHidden--)| boolean | Indicates whether the object is visible. |
| [isLockAspectRatio](#isLockAspectRatio--)| boolean | True means that aspect ratio of the shape is locked. |
| [isAspectRatioLocked](#isAspectRatioLocked--)| boolean | True means that aspect ratio of the shape is locked. |
| [rotationAngle](#rotationAngle--)| number | Gets and sets the rotation of the shape. |
| [hyperlink](#hyperlink--)| Hyperlink | Readonly. Gets the hyperlink of the shape. |
| [id](#id--)| number | Readonly. Gets the identifier of this shape. |
| [spid](#spid--)| string | Readonly. Specifies an optional string identifier that an application can use to identify the particular shape. |
| [spt](#spt--)| number | Readonly. Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the [Worksheet](../worksheet/) object which contains this shape. |
| [isGroup](#isGroup--)| boolean | Readonly. Indicates whether this shape is a group shape. |
| [isInGroup](#isInGroup--)| boolean | Readonly. Indicates whether the shape is grouped. |
| [isWordArt](#isWordArt--)| boolean | Readonly. Indicates whether this shape is a word art. |
| [textEffect](#textEffect--)| TextEffectFormat | Readonly. Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt. |
| [isLocked](#isLocked--)| boolean | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [isPrintable](#isPrintable--)| boolean | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [msoDrawingType](#msoDrawingType--)| MsoDrawingType | Readonly. Gets drawing type. |
| [autoShapeType](#autoShapeType--)| AutoShapeType | Gets and sets the auto shape type. |
| [anchorType](#anchorType--)| ShapeAnchorType | Gets and set the type of the shape anchor placeholder. |
| [placement](#placement--)| PlacementType | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [upperLeftRow](#upperLeftRow--)| number | Represents the top row index. |
| [upperDeltaY](#upperDeltaY--)| number | Gets or sets the shape's vertical offset from its upper left corner row. |
| [upperLeftColumn](#upperLeftColumn--)| number | Represents upper left corner column index. |
| [upperDeltaX](#upperDeltaX--)| number | Gets or sets the shape's horizontal offset from its upper left corner column. |
| [lowerRightRow](#lowerRightRow--)| number | Represents lower right corner row index. |
| [lowerDeltaY](#lowerDeltaY--)| number | Gets or sets the shape's vertical offset from its lower right corner row. |
| [lowerRightColumn](#lowerRightColumn--)| number | Represents lower right corner column index. |
| [lowerDeltaX](#lowerDeltaX--)| number | Gets or sets the shape's horizontal  offset from its lower right corner column. |
| [right](#right--)| number | Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
| [bottom](#bottom--)| number | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [width](#width--)| number | Represents the width of shape, in unit of pixels. |
| [widthInch](#widthInch--)| number | Represents the width of the shape, in unit of inch. |
| [widthPt](#widthPt--)| number | Represents the width of the shape, in unit of point. |
| [widthCM](#widthCM--)| number | Represents the width of the shape, in unit of centimeters. |
| [height](#height--)| number | Represents the height of shape, in unit of pixel. |
| [heightInch](#heightInch--)| number | Represents the height of the shape, in unit of inches. |
| [heightPt](#heightPt--)| number | Represents the height of the shape, in unit of points. |
| [heightCM](#heightCM--)| number | Represents the height of the shape, in unit of centimeters. |
| [left](#left--)| number | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [leftInch](#leftInch--)| number | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [leftCM](#leftCM--)| number | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [top](#top--)| number | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [topInch](#topInch--)| number | Represents the vertical offset of shape from its top row, in unit of inches. |
| [topCM](#topCM--)| number | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [topToCorner](#topToCorner--)| number | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [leftToCorner](#leftToCorner--)| number | Gets and sets the horizonal offset of shape from worksheet left border. |
| [x](#x--)| number | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [y](#y--)| number | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [widthScale](#widthScale--)| number | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100; |
| [heightScale](#heightScale--)| number | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100; |
| [topInShape](#topInShape--)| number | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [leftInShape](#leftInShape--)| number | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [widthInShape](#widthInShape--)| number | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [heightInShape](#heightInShape--)| number | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [group](#group--)| GroupShape | Readonly. Gets the group shape which contains this shape. |
| [type](#type--)| AutoShapeType | Readonly. Gets the auto shape type. |
| [hasLine](#hasLine--)| boolean | Gets and sets the line border of the shape is visible. |
| [isFilled](#isFilled--)| boolean | Indicates whether the fill format is visible. |
| [isFlippedHorizontally](#isFlippedHorizontally--)| boolean | Gets and sets whether shape is horizontally flipped . |
| [isFlippedVertically](#isFlippedVertically--)| boolean | Gets and sets whether shape is vertically flipped . |
| [actualLowerRightRow](#actualLowerRightRow--)| number | Readonly. Get the actual bottom row. |
| [relativeToOriginalPictureSize](#relativeToOriginalPictureSize--)| boolean | Indicates whether shape is relative to original picture size. |
| [linkedCell](#linkedCell--)| string | Gets or sets the worksheet range linked to the control's value. |
| [inputRange](#inputRange--)| string | Gets or sets the worksheet range used to fill the specified combo box. |
| [textShapeType](#textShapeType--)| AutoShapeType | Gets and sets the preset text shape type. |
| [textBody](#textBody--)| FontSettingCollection | Readonly. Gets and sets the setting of the shape's text. |
| [font](#font--)| Font | Represents the font of shape. |
| [textOptions](#textOptions--)| TextOptions | Represents the text options of the shape. |
| [text](#text--)| string | Gets and sets the text of this shape. |
| [isRichText](#isRichText--)| boolean | Readonly. Whether or not the text is rich text. |
| [htmlText](#htmlText--)| string | Gets and sets the html string which contains data and some formats in this textbox. |
| [textVerticalOverflow](#textVerticalOverflow--)| TextOverflowType | Gets and sets the text vertical overflow type of the shape which contains text. |
| [textHorizontalOverflow](#textHorizontalOverflow--)| TextOverflowType | Gets and sets the text horizontal overflow type of the shape which contains text. |
| [isTextWrapped](#isTextWrapped--)| boolean | Gets and sets the text wrapped type of the shape which contains text. |
| [textOrientationType](#textOrientationType--)| TextOrientationType | Gets and sets the text orientation type of the shape. |
| [textHorizontalAlignment](#textHorizontalAlignment--)| TextAlignmentType | Gets and sets the text horizontal alignment type of the shape. |
| [textVerticalAlignment](#textVerticalAlignment--)| TextAlignmentType | Gets and sets the text vertical alignment type of the shape. |
| [textDirection](#textDirection--)| TextDirectionType | Gets/Sets the direction of the text flow for this object. |
| [textBoxOptions](#textBoxOptions--)| TextBoxOptions | Readonly. Gets the text information in the shape |
| [controlData](#controlData--)| Uint8Array | Readonly. Gets the data of control. |
| [activeXControl](#activeXControl--)| ActiveXControl | Readonly. Gets the ActiveX control. |
| [paths](#paths--)| ShapePathCollection | Readonly. Gets the paths of a custom geometric shape. |
| [geometry](#geometry--)| Geometry | Readonly. Gets the geometry |
| [isDecorative](#isDecorative--)| boolean | Indicates whether the object is decorative. |

## Methods

| Method | Description |
| --- | --- |
| [isAutoSize()](#isAutoSize--)| <b>@deprecated.</b> Please use the 'isAutoSize' property instead. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated. |
| [setIsAutoSize(boolean)](#setIsAutoSize-boolean-)| <b>@deprecated.</b> Please use the 'isAutoSize' property instead. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated. |
| [isLink()](#isLink--)| <b>@deprecated.</b> Please use the 'isLink' property instead. Returns true if the OleObject links to the file. |
| [set_IsLink(boolean)](#set_IsLink-boolean-)| <b>@deprecated.</b> Please use the 'isLink' property instead. Returns true if the OleObject links to the file. |
| [getDisplayAsIcon()](#getDisplayAsIcon--)| <b>@deprecated.</b> Please use the 'displayAsIcon' property instead. True if the specified object is displayed as an icon and the image will not be auto changed. |
| [setDisplayAsIcon(boolean)](#setDisplayAsIcon-boolean-)| <b>@deprecated.</b> Please use the 'displayAsIcon' property instead. True if the specified object is displayed as an icon and the image will not be auto changed. |
| [getImageData()](#getImageData--)| <b>@deprecated.</b> Please use the 'imageData' property instead. Represents image of ole object as byte array. |
| [setImageData(Uint8Array)](#setImageData-uint8array-)| <b>@deprecated.</b> Please use the 'imageData' property instead. Represents image of ole object as byte array. |
| [getObjectData()](#getObjectData--)| <b>@deprecated.</b> Please use the 'objectData' property instead. Represents embedded ole object data as byte array. |
| [setObjectData(Uint8Array)](#setObjectData-uint8array-)| <b>@deprecated.</b> Please use the 'objectData' property instead. Represents embedded ole object data as byte array. |
| [getFullObjectBin()](#getFullObjectBin--)| <b>@deprecated.</b> Please use the 'fullObjectBin' property instead. Gets the full embedded ole object binary data in the template file. |
| [getImageSourceFullName()](#getImageSourceFullName--)| <b>@deprecated.</b> Please use the 'imageSourceFullName' property instead. Gets or sets the path and name of the source file for the linked image. |
| [setImageSourceFullName(string)](#setImageSourceFullName-string-)| <b>@deprecated.</b> Please use the 'imageSourceFullName' property instead. Gets or sets the path and name of the source file for the linked image. |
| [getProgID()](#getProgID--)| <b>@deprecated.</b> Please use the 'progID' property instead. Gets or sets the ProgID of the OLE object. |
| [setProgID(string)](#setProgID-string-)| <b>@deprecated.</b> Please use the 'progID' property instead. Gets or sets the ProgID of the OLE object. |
| [getFileFormatType()](#getFileFormatType--)| <b>@deprecated.</b> Please use the 'fileFormatType' property instead. Gets and sets the file type of the embedded ole object data |
| [setFileFormatType(FileFormatType)](#setFileFormatType-fileformattype-)| <b>@deprecated.</b> Please use the 'fileFormatType' property instead. Gets and sets the file type of the embedded ole object data |
| [getObjectSourceFullName()](#getObjectSourceFullName--)| <b>@deprecated.</b> Please use the 'objectSourceFullName' property instead. Returns the source full name of the source file for the linked OLE object. |
| [setObjectSourceFullName(string)](#setObjectSourceFullName-string-)| <b>@deprecated.</b> Please use the 'objectSourceFullName' property instead. Returns the source full name of the source file for the linked OLE object. |
| [getLabel()](#getLabel--)| <b>@deprecated.</b> Please use the 'label' property instead. Gets and sets the display label of the linked ole object. |
| [setLabel(string)](#setLabel-string-)| <b>@deprecated.</b> Please use the 'label' property instead. Gets and sets the display label of the linked ole object. |
| [getAutoUpdate()](#getAutoUpdate--)| <b>@deprecated.</b> Please use the 'autoUpdate' property instead. Specifies whether the link to the OleObject is automatically updated or not. |
| [setAutoUpdate(boolean)](#setAutoUpdate-boolean-)| <b>@deprecated.</b> Please use the 'autoUpdate' property instead. Specifies whether the link to the OleObject is automatically updated or not. |
| [getAutoLoad()](#getAutoLoad--)| <b>@deprecated.</b> Please use the 'autoLoad' property instead. Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened. |
| [setAutoLoad(boolean)](#setAutoLoad-boolean-)| <b>@deprecated.</b> Please use the 'autoLoad' property instead. Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened. |
| [getClassIdentifier()](#getClassIdentifier--)| <b>@deprecated.</b> Please use the 'classIdentifier' property instead. Gets and sets the class identifier of the embedded object. It means which application opens the embedded file. |
| [setClassIdentifier(Uint8Array)](#setClassIdentifier-uint8array-)| <b>@deprecated.</b> Please use the 'classIdentifier' property instead. Gets and sets the class identifier of the embedded object. It means which application opens the embedded file. |
| [getImageType()](#getImageType--)| <b>@deprecated.</b> Please use the 'imageType' property instead. Gets the image format of the ole object. |
| [setEmbeddedObject(boolean, Uint8Array, string, boolean, string)](#setEmbeddedObject-boolean-uint8array-string-boolean-string-)| Sets embedded object data. |
| [setEmbeddedObject(boolean, Uint8Array, string, boolean, string, boolean)](#setEmbeddedObject-boolean-uint8array-string-boolean-string-boolean-)| Sets embedded object data. |
| [setNativeSourceFullName(string)](#setNativeSourceFullName-string-)| Sets the ole native source full file name with path. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getMacroName()](#getMacroName--)| <b>@deprecated.</b> Please use the 'macroName' property instead. Gets and sets the name of macro. |
| [setMacroName(string)](#setMacroName-string-)| <b>@deprecated.</b> Please use the 'macroName' property instead. Gets and sets the name of macro. |
| [isEquation()](#isEquation--)| <b>@deprecated.</b> Please use the 'isEquation' property instead. Indicates whether the shape only contains an equation. |
| [isSmartArt()](#isSmartArt--)| <b>@deprecated.</b> Please use the 'isSmartArt' property instead. Indicates whether the shape is a smart art. |
| [getZOrderPosition()](#getZOrderPosition--)| <b>@deprecated.</b> Please use the 'zOrderPosition' property instead. Returns the position of a shape in the z-order. |
| [setZOrderPosition(number)](#setZOrderPosition-number-)| <b>@deprecated.</b> Please use the 'zOrderPosition' property instead. Returns the position of a shape in the z-order. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the shape. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the shape. |
| [getAlternativeText()](#getAlternativeText--)| <b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object. |
| [setAlternativeText(string)](#setAlternativeText-string-)| <b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object. |
| [getTitle()](#getTitle--)| <b>@deprecated.</b> Please use the 'title' property instead. Specifies the title (caption) of the current shape object. |
| [setTitle(string)](#setTitle-string-)| <b>@deprecated.</b> Please use the 'title' property instead. Specifies the title (caption) of the current shape object. |
| [getLine()](#getLine--)| <b>@deprecated.</b> Please use the 'line' property instead. Gets line style |
| [getFill()](#getFill--)| <b>@deprecated.</b> Please use the 'fill' property instead. Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape. |
| [getShadowEffect()](#getShadowEffect--)| <b>@deprecated.</b> Please use the 'shadowEffect' property instead. Represents a [Drawing.ShadowEffect](../drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [getReflection()](#getReflection--)| <b>@deprecated.</b> Please use the 'reflection' property instead. Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape. |
| [getGlow()](#getGlow--)| <b>@deprecated.</b> Please use the 'glow' property instead. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape. |
| [getSoftEdges()](#getSoftEdges--)| <b>@deprecated.</b> Please use the 'softEdges' property instead. Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [setSoftEdges(number)](#setSoftEdges-number-)| <b>@deprecated.</b> Please use the 'softEdges' property instead. Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [getThreeDFormat()](#getThreeDFormat--)| <b>@deprecated.</b> Please use the 'threeDFormat' property instead. Gets and sets 3d format of the shape. |
| [getFormatPicture()](#getFormatPicture--)| <b>@deprecated.</b> Please use the 'formatPicture' property instead. Gets and sets the options of the picture format. |
| [isHidden()](#isHidden--)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether the object is visible. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether the object is visible. |
| [isLockAspectRatio()](#isLockAspectRatio--)| <b>@deprecated.</b> Please use the 'isLockAspectRatio' property instead. True means that aspect ratio of the shape is locked. |
| [setIsLockAspectRatio(boolean)](#setIsLockAspectRatio-boolean-)| <b>@deprecated.</b> Please use the 'isLockAspectRatio' property instead. True means that aspect ratio of the shape is locked. |
| [isAspectRatioLocked()](#isAspectRatioLocked--)| <b>@deprecated.</b> Please use the 'isAspectRatioLocked' property instead. True means that aspect ratio of the shape is locked. |
| [setIsAspectRatioLocked(boolean)](#setIsAspectRatioLocked-boolean-)| <b>@deprecated.</b> Please use the 'isAspectRatioLocked' property instead. True means that aspect ratio of the shape is locked. |
| [getRotationAngle()](#getRotationAngle--)| <b>@deprecated.</b> Please use the 'rotationAngle' property instead. Gets and sets the rotation of the shape. |
| [setRotationAngle(number)](#setRotationAngle-number-)| <b>@deprecated.</b> Please use the 'rotationAngle' property instead. Gets and sets the rotation of the shape. |
| [getHyperlink()](#getHyperlink--)| <b>@deprecated.</b> Please use the 'hyperlink' property instead. Gets the hyperlink of the shape. |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets the identifier of this shape. |
| [getSpid()](#getSpid--)| <b>@deprecated.</b> Please use the 'spid' property instead. Specifies an optional string identifier that an application can use to identify the particular shape. |
| [getSpt()](#getSpt--)| <b>@deprecated.</b> Please use the 'spt' property instead. Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the [Worksheet](../worksheet/) object which contains this shape. |
| [isGroup()](#isGroup--)| <b>@deprecated.</b> Please use the 'isGroup' property instead. Indicates whether this shape is a group shape. |
| [isInGroup()](#isInGroup--)| <b>@deprecated.</b> Please use the 'isInGroup' property instead. Indicates whether the shape is grouped. |
| [isWordArt()](#isWordArt--)| <b>@deprecated.</b> Please use the 'isWordArt' property instead. Indicates whether this shape is a word art. |
| [getTextEffect()](#getTextEffect--)| <b>@deprecated.</b> Please use the 'textEffect' property instead. Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt. |
| [isLocked()](#isLocked--)| <b>@deprecated.</b> Please use the 'isLocked' property instead. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| <b>@deprecated.</b> Please use the 'isLocked' property instead. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [isPrintable()](#isPrintable--)| <b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [setIsPrintable(boolean)](#setIsPrintable-boolean-)| <b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [getMsoDrawingType()](#getMsoDrawingType--)| <b>@deprecated.</b> Please use the 'msoDrawingType' property instead. Gets drawing type. |
| [getAutoShapeType()](#getAutoShapeType--)| <b>@deprecated.</b> Please use the 'autoShapeType' property instead. Gets and sets the auto shape type. |
| [setAutoShapeType(AutoShapeType)](#setAutoShapeType-autoshapetype-)| <b>@deprecated.</b> Please use the 'autoShapeType' property instead. Gets and sets the auto shape type. |
| [getAnchorType()](#getAnchorType--)| <b>@deprecated.</b> Please use the 'anchorType' property instead. Gets and set the type of the shape anchor placeholder. |
| [setAnchorType(ShapeAnchorType)](#setAnchorType-shapeanchortype-)| <b>@deprecated.</b> Please use the 'anchorType' property instead. Gets and set the type of the shape anchor placeholder. |
| [getPlacement()](#getPlacement--)| <b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [setPlacement(PlacementType)](#setPlacement-placementtype-)| <b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [getUpperLeftRow()](#getUpperLeftRow--)| <b>@deprecated.</b> Please use the 'upperLeftRow' property instead. Represents the top row index. |
| [setUpperLeftRow(number)](#setUpperLeftRow-number-)| <b>@deprecated.</b> Please use the 'upperLeftRow' property instead. Represents the top row index. |
| [getUpperDeltaY()](#getUpperDeltaY--)| <b>@deprecated.</b> Please use the 'upperDeltaY' property instead. Gets or sets the shape's vertical offset from its upper left corner row. |
| [setUpperDeltaY(number)](#setUpperDeltaY-number-)| <b>@deprecated.</b> Please use the 'upperDeltaY' property instead. Gets or sets the shape's vertical offset from its upper left corner row. |
| [getUpperLeftColumn()](#getUpperLeftColumn--)| <b>@deprecated.</b> Please use the 'upperLeftColumn' property instead. Represents upper left corner column index. |
| [setUpperLeftColumn(number)](#setUpperLeftColumn-number-)| <b>@deprecated.</b> Please use the 'upperLeftColumn' property instead. Represents upper left corner column index. |
| [getUpperDeltaX()](#getUpperDeltaX--)| <b>@deprecated.</b> Please use the 'upperDeltaX' property instead. Gets or sets the shape's horizontal offset from its upper left corner column. |
| [setUpperDeltaX(number)](#setUpperDeltaX-number-)| <b>@deprecated.</b> Please use the 'upperDeltaX' property instead. Gets or sets the shape's horizontal offset from its upper left corner column. |
| [getLowerRightRow()](#getLowerRightRow--)| <b>@deprecated.</b> Please use the 'lowerRightRow' property instead. Represents lower right corner row index. |
| [setLowerRightRow(number)](#setLowerRightRow-number-)| <b>@deprecated.</b> Please use the 'lowerRightRow' property instead. Represents lower right corner row index. |
| [getLowerDeltaY()](#getLowerDeltaY--)| <b>@deprecated.</b> Please use the 'lowerDeltaY' property instead. Gets or sets the shape's vertical offset from its lower right corner row. |
| [setLowerDeltaY(number)](#setLowerDeltaY-number-)| <b>@deprecated.</b> Please use the 'lowerDeltaY' property instead. Gets or sets the shape's vertical offset from its lower right corner row. |
| [getLowerRightColumn()](#getLowerRightColumn--)| <b>@deprecated.</b> Please use the 'lowerRightColumn' property instead. Represents lower right corner column index. |
| [setLowerRightColumn(number)](#setLowerRightColumn-number-)| <b>@deprecated.</b> Please use the 'lowerRightColumn' property instead. Represents lower right corner column index. |
| [getLowerDeltaX()](#getLowerDeltaX--)| <b>@deprecated.</b> Please use the 'lowerDeltaX' property instead. Gets or sets the shape's horizontal  offset from its lower right corner column. |
| [setLowerDeltaX(number)](#setLowerDeltaX-number-)| <b>@deprecated.</b> Please use the 'lowerDeltaX' property instead. Gets or sets the shape's horizontal  offset from its lower right corner column. |
| [getRight()](#getRight--)| <b>@deprecated.</b> Please use the 'right' property instead. Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
| [setRight(number)](#setRight-number-)| <b>@deprecated.</b> Please use the 'right' property instead. Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
| [getBottom()](#getBottom--)| <b>@deprecated.</b> Please use the 'bottom' property instead. Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [setBottom(number)](#setBottom-number-)| <b>@deprecated.</b> Please use the 'bottom' property instead. Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [getWidth()](#getWidth--)| <b>@deprecated.</b> Please use the 'width' property instead. Represents the width of shape, in unit of pixels. |
| [setWidth(number)](#setWidth-number-)| <b>@deprecated.</b> Please use the 'width' property instead. Represents the width of shape, in unit of pixels. |
| [getWidthInch()](#getWidthInch--)| <b>@deprecated.</b> Please use the 'widthInch' property instead. Represents the width of the shape, in unit of inch. |
| [setWidthInch(number)](#setWidthInch-number-)| <b>@deprecated.</b> Please use the 'widthInch' property instead. Represents the width of the shape, in unit of inch. |
| [getWidthPt()](#getWidthPt--)| <b>@deprecated.</b> Please use the 'widthPt' property instead. Represents the width of the shape, in unit of point. |
| [setWidthPt(number)](#setWidthPt-number-)| <b>@deprecated.</b> Please use the 'widthPt' property instead. Represents the width of the shape, in unit of point. |
| [getWidthCM()](#getWidthCM--)| <b>@deprecated.</b> Please use the 'widthCM' property instead. Represents the width of the shape, in unit of centimeters. |
| [setWidthCM(number)](#setWidthCM-number-)| <b>@deprecated.</b> Please use the 'widthCM' property instead. Represents the width of the shape, in unit of centimeters. |
| [getHeight()](#getHeight--)| <b>@deprecated.</b> Please use the 'height' property instead. Represents the height of shape, in unit of pixel. |
| [setHeight(number)](#setHeight-number-)| <b>@deprecated.</b> Please use the 'height' property instead. Represents the height of shape, in unit of pixel. |
| [getHeightInch()](#getHeightInch--)| <b>@deprecated.</b> Please use the 'heightInch' property instead. Represents the height of the shape, in unit of inches. |
| [setHeightInch(number)](#setHeightInch-number-)| <b>@deprecated.</b> Please use the 'heightInch' property instead. Represents the height of the shape, in unit of inches. |
| [getHeightPt()](#getHeightPt--)| <b>@deprecated.</b> Please use the 'heightPt' property instead. Represents the height of the shape, in unit of points. |
| [setHeightPt(number)](#setHeightPt-number-)| <b>@deprecated.</b> Please use the 'heightPt' property instead. Represents the height of the shape, in unit of points. |
| [getHeightCM()](#getHeightCM--)| <b>@deprecated.</b> Please use the 'heightCM' property instead. Represents the height of the shape, in unit of centimeters. |
| [setHeightCM(number)](#setHeightCM-number-)| <b>@deprecated.</b> Please use the 'heightCM' property instead. Represents the height of the shape, in unit of centimeters. |
| [getLeft()](#getLeft--)| <b>@deprecated.</b> Please use the 'left' property instead. Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [setLeft(number)](#setLeft-number-)| <b>@deprecated.</b> Please use the 'left' property instead. Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftInch()](#getLeftInch--)| <b>@deprecated.</b> Please use the 'leftInch' property instead. Represents the horizontal offset of shape from its left column, in unit of inches. |
| [setLeftInch(number)](#setLeftInch-number-)| <b>@deprecated.</b> Please use the 'leftInch' property instead. Represents the horizontal offset of shape from its left column, in unit of inches. |
| [getLeftCM()](#getLeftCM--)| <b>@deprecated.</b> Please use the 'leftCM' property instead. Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [setLeftCM(number)](#setLeftCM-number-)| <b>@deprecated.</b> Please use the 'leftCM' property instead. Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [getTop()](#getTop--)| <b>@deprecated.</b> Please use the 'top' property instead. Represents the vertical offset of shape from its top row, in unit of pixels. |
| [setTop(number)](#setTop-number-)| <b>@deprecated.</b> Please use the 'top' property instead. Represents the vertical offset of shape from its top row, in unit of pixels. |
| [getTopInch()](#getTopInch--)| <b>@deprecated.</b> Please use the 'topInch' property instead. Represents the vertical offset of shape from its top row, in unit of inches. |
| [setTopInch(number)](#setTopInch-number-)| <b>@deprecated.</b> Please use the 'topInch' property instead. Represents the vertical offset of shape from its top row, in unit of inches. |
| [getTopCM()](#getTopCM--)| <b>@deprecated.</b> Please use the 'topCM' property instead. Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [setTopCM(number)](#setTopCM-number-)| <b>@deprecated.</b> Please use the 'topCM' property instead. Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [getTopToCorner()](#getTopToCorner--)| <b>@deprecated.</b> Please use the 'topToCorner' property instead. Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [setTopToCorner(number)](#setTopToCorner-number-)| <b>@deprecated.</b> Please use the 'topToCorner' property instead. Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [getLeftToCorner()](#getLeftToCorner--)| <b>@deprecated.</b> Please use the 'leftToCorner' property instead. Gets and sets the horizonal offset of shape from worksheet left border. |
| [setLeftToCorner(number)](#setLeftToCorner-number-)| <b>@deprecated.</b> Please use the 'leftToCorner' property instead. Gets and sets the horizonal offset of shape from worksheet left border. |
| [getX()](#getX--)| <b>@deprecated.</b> Please use the 'x' property instead. Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [setX(number)](#setX-number-)| <b>@deprecated.</b> Please use the 'x' property instead. Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [getY()](#getY--)| <b>@deprecated.</b> Please use the 'y' property instead. Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [setY(number)](#setY-number-)| <b>@deprecated.</b> Please use the 'y' property instead. Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getWidthScale()](#getWidthScale--)| <b>@deprecated.</b> Please use the 'widthScale' property instead. Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100; |
| [setWidthScale(number)](#setWidthScale-number-)| <b>@deprecated.</b> Please use the 'widthScale' property instead. Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100; |
| [getHeightScale()](#getHeightScale--)| <b>@deprecated.</b> Please use the 'heightScale' property instead. Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100; |
| [setHeightScale(number)](#setHeightScale-number-)| <b>@deprecated.</b> Please use the 'heightScale' property instead. Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100; |
| [getTopInShape()](#getTopInShape--)| <b>@deprecated.</b> Please use the 'topInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [setTopInShape(number)](#setTopInShape-number-)| <b>@deprecated.</b> Please use the 'topInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [getLeftInShape()](#getLeftInShape--)| <b>@deprecated.</b> Please use the 'leftInShape' property instead. Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [setLeftInShape(number)](#setLeftInShape-number-)| <b>@deprecated.</b> Please use the 'leftInShape' property instead. Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [getWidthInShape()](#getWidthInShape--)| <b>@deprecated.</b> Please use the 'widthInShape' property instead. Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [setWidthInShape(number)](#setWidthInShape-number-)| <b>@deprecated.</b> Please use the 'widthInShape' property instead. Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [getHeightInShape()](#getHeightInShape--)| <b>@deprecated.</b> Please use the 'heightInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [setHeightInShape(number)](#setHeightInShape-number-)| <b>@deprecated.</b> Please use the 'heightInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [getGroup()](#getGroup--)| <b>@deprecated.</b> Please use the 'group' property instead. Gets the group shape which contains this shape. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the auto shape type. |
| [getHasLine()](#getHasLine--)| <b>@deprecated.</b> Please use the 'hasLine' property instead. Gets and sets the line border of the shape is visible. |
| [setHasLine(boolean)](#setHasLine-boolean-)| <b>@deprecated.</b> Please use the 'hasLine' property instead. Gets and sets the line border of the shape is visible. |
| [isFilled()](#isFilled--)| <b>@deprecated.</b> Please use the 'isFilled' property instead. Indicates whether the fill format is visible. |
| [setIsFilled(boolean)](#setIsFilled-boolean-)| <b>@deprecated.</b> Please use the 'isFilled' property instead. Indicates whether the fill format is visible. |
| [isFlippedHorizontally()](#isFlippedHorizontally--)| <b>@deprecated.</b> Please use the 'isFlippedHorizontally' property instead. Gets and sets whether shape is horizontally flipped . |
| [setIsFlippedHorizontally(boolean)](#setIsFlippedHorizontally-boolean-)| <b>@deprecated.</b> Please use the 'isFlippedHorizontally' property instead. Gets and sets whether shape is horizontally flipped . |
| [isFlippedVertically()](#isFlippedVertically--)| <b>@deprecated.</b> Please use the 'isFlippedVertically' property instead. Gets and sets whether shape is vertically flipped . |
| [setIsFlippedVertically(boolean)](#setIsFlippedVertically-boolean-)| <b>@deprecated.</b> Please use the 'isFlippedVertically' property instead. Gets and sets whether shape is vertically flipped . |
| [getActualLowerRightRow()](#getActualLowerRightRow--)| <b>@deprecated.</b> Please use the 'actualLowerRightRow' property instead. Get the actual bottom row. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--)| <b>@deprecated.</b> Please use the 'relativeToOriginalPictureSize' property instead. Indicates whether shape is relative to original picture size. |
| [setRelativeToOriginalPictureSize(boolean)](#setRelativeToOriginalPictureSize-boolean-)| <b>@deprecated.</b> Please use the 'relativeToOriginalPictureSize' property instead. Indicates whether shape is relative to original picture size. |
| [getLinkedCell()](#getLinkedCell--)| <b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets or sets the worksheet range linked to the control's value. |
| [setLinkedCell(string)](#setLinkedCell-string-)| <b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets or sets the worksheet range linked to the control's value. |
| [getInputRange()](#getInputRange--)| <b>@deprecated.</b> Please use the 'inputRange' property instead. Gets or sets the worksheet range used to fill the specified combo box. |
| [setInputRange(string)](#setInputRange-string-)| <b>@deprecated.</b> Please use the 'inputRange' property instead. Gets or sets the worksheet range used to fill the specified combo box. |
| [getTextShapeType()](#getTextShapeType--)| <b>@deprecated.</b> Please use the 'textShapeType' property instead. Gets and sets the preset text shape type. |
| [setTextShapeType(AutoShapeType)](#setTextShapeType-autoshapetype-)| <b>@deprecated.</b> Please use the 'textShapeType' property instead. Gets and sets the preset text shape type. |
| [getTextBody()](#getTextBody--)| <b>@deprecated.</b> Please use the 'textBody' property instead. Gets and sets the setting of the shape's text. |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Represents the font of shape. |
| [setFont(Font)](#setFont-font-)| <b>@deprecated.</b> Please use the 'font' property instead. Represents the font of shape. |
| [getTextOptions()](#getTextOptions--)| <b>@deprecated.</b> Please use the 'textOptions' property instead. Represents the text options of the shape. |
| [setTextOptions(TextOptions)](#setTextOptions-textoptions-)| <b>@deprecated.</b> Please use the 'textOptions' property instead. Represents the text options of the shape. |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. Gets and sets the text of this shape. |
| [setText(string)](#setText-string-)| <b>@deprecated.</b> Please use the 'text' property instead. Gets and sets the text of this shape. |
| [isRichText()](#isRichText--)| <b>@deprecated.</b> Please use the 'isRichText' property instead. Whether or not the text is rich text. |
| [getHtmlText()](#getHtmlText--)| <b>@deprecated.</b> Please use the 'htmlText' property instead. Gets and sets the html string which contains data and some formats in this textbox. |
| [setHtmlText(string)](#setHtmlText-string-)| <b>@deprecated.</b> Please use the 'htmlText' property instead. Gets and sets the html string which contains data and some formats in this textbox. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--)| <b>@deprecated.</b> Please use the 'textVerticalOverflow' property instead. Gets and sets the text vertical overflow type of the shape which contains text. |
| [setTextVerticalOverflow(TextOverflowType)](#setTextVerticalOverflow-textoverflowtype-)| <b>@deprecated.</b> Please use the 'textVerticalOverflow' property instead. Gets and sets the text vertical overflow type of the shape which contains text. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--)| <b>@deprecated.</b> Please use the 'textHorizontalOverflow' property instead. Gets and sets the text horizontal overflow type of the shape which contains text. |
| [setTextHorizontalOverflow(TextOverflowType)](#setTextHorizontalOverflow-textoverflowtype-)| <b>@deprecated.</b> Please use the 'textHorizontalOverflow' property instead. Gets and sets the text horizontal overflow type of the shape which contains text. |
| [isTextWrapped()](#isTextWrapped--)| <b>@deprecated.</b> Please use the 'isTextWrapped' property instead. Gets and sets the text wrapped type of the shape which contains text. |
| [setIsTextWrapped(boolean)](#setIsTextWrapped-boolean-)| <b>@deprecated.</b> Please use the 'isTextWrapped' property instead. Gets and sets the text wrapped type of the shape which contains text. |
| [getTextOrientationType()](#getTextOrientationType--)| <b>@deprecated.</b> Please use the 'textOrientationType' property instead. Gets and sets the text orientation type of the shape. |
| [setTextOrientationType(TextOrientationType)](#setTextOrientationType-textorientationtype-)| <b>@deprecated.</b> Please use the 'textOrientationType' property instead. Gets and sets the text orientation type of the shape. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--)| <b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment type of the shape. |
| [setTextHorizontalAlignment(TextAlignmentType)](#setTextHorizontalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment type of the shape. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--)| <b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets and sets the text vertical alignment type of the shape. |
| [setTextVerticalAlignment(TextAlignmentType)](#setTextVerticalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets and sets the text vertical alignment type of the shape. |
| [getTextDirection()](#getTextDirection--)| <b>@deprecated.</b> Please use the 'textDirection' property instead. Gets/Sets the direction of the text flow for this object. |
| [setTextDirection(TextDirectionType)](#setTextDirection-textdirectiontype-)| <b>@deprecated.</b> Please use the 'textDirection' property instead. Gets/Sets the direction of the text flow for this object. |
| [getTextBoxOptions()](#getTextBoxOptions--)| <b>@deprecated.</b> Please use the 'textBoxOptions' property instead. Gets the text information in the shape |
| [getControlData()](#getControlData--)| <b>@deprecated.</b> Please use the 'controlData' property instead. Gets the data of control. |
| [getActiveXControl()](#getActiveXControl--)| <b>@deprecated.</b> Please use the 'activeXControl' property instead. Gets the ActiveX control. |
| [getPaths()](#getPaths--)| <b>@deprecated.</b> Please use the 'paths' property instead. Gets the paths of a custom geometric shape. |
| [getGeometry()](#getGeometry--)| <b>@deprecated.</b> Please use the 'geometry' property instead. Gets the geometry |
| [isDecorative()](#isDecorative--)| <b>@deprecated.</b> Please use the 'isDecorative' property instead. Indicates whether the object is decorative. |
| [setIsDecorative(boolean)](#setIsDecorative-boolean-)| <b>@deprecated.</b> Please use the 'isDecorative' property instead. Indicates whether the object is decorative. |
| [toFrontOrBack(number)](#toFrontOrBack-number-)| Brings the shape to the front or sends the shape to back. |
| [getLockedProperty(ShapeLockType)](#getLockedProperty-shapelocktype-)| Gets the value of locked property. |
| [setLockedProperty(ShapeLockType, boolean)](#setLockedProperty-shapelocktype-boolean-)| Set the locked property. |
| [addHyperlink(string)](#addHyperlink-string-)| Adds a hyperlink to the shape. |
| [removeHyperlink()](#removeHyperlink--)| Removes the hyperlink of the shape. |
| [moveToRange(number, number, number, number)](#moveToRange-number-number-number-number-)| Moves the shape to a specified range. |
| [alignTopRightCorner(number, number)](#alignTopRightCorner-number-number-)| Moves the picture to the top-right corner. |
| [getConnectionPoints()](#getConnectionPoints--)| Get the connection points |
| [toImage(ImageType)](#toImage-imagetype-)| Creates the shape image and saves it to a stream in the specified format. |
| [toImage(string, ImageOrPrintOptions)](#toImage-string-imageorprintoptions-)| Saves the shape to a file. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Saves the shape to a stream. |
| [toImageAsync(ImageType)](#toImageAsync-imagetype-)| Creates the shape image and saves it to a stream in the specified format. |
| [toImageAsync(string, ImageOrPrintOptions)](#toImageAsync-string-imageorprintoptions-)| Saves the shape to a file. |
| [toImageAsync(ImageOrPrintOptions)](#toImageAsync-imageorprintoptions-)| Saves the shape to a stream. |
| [getLinkedCell(boolean, boolean)](#getLinkedCell-boolean-boolean-)| Gets the range linked to the control's value. |
| [setLinkedCell(string, boolean, boolean)](#setLinkedCell-string-boolean-boolean-)| Sets the range linked to the control's value. |
| [getInputRange(boolean, boolean)](#getInputRange-boolean-boolean-)| Gets the range used to fill the control. |
| [setInputRange(string, boolean, boolean)](#setInputRange-string-boolean-boolean-)| Sets the range used to fill the control. |
| [updateSelectedValue()](#updateSelectedValue--)| Update the selected value by the value of the linked cell. |
| [calculateTextSize()](#calculateTextSize--)| Recalculate the text area |
| [formatCharacters(number, number, Font, StyleFlag)](#formatCharacters-number-number-font-styleflag-)| Formats some characters with the font setting. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the text. |
| [getRichFormattings()](#getRichFormattings--)| Returns all Characters objects that represents a range of characters within the text . |
| [removeActiveXControl()](#removeActiveXControl--)| Remove activeX control. |
| [getActualBox()](#getActualBox--)| Get the actual position and size of the shape (after applying rotation, flip, etc.) |
| [fitToTextSize()](#fitToTextSize--)| Recalculate a text area suitable for displaying all text content. |
| [getResultOfSmartArt()](#getResultOfSmartArt--)| Converting smart art to grouped shapes. |
| [isSameSetting(Object)](#isSameSetting-object-)| Returns whether the shape is same. |


### constructor(Shape) {#constructor-shape-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Shape);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Shape | The parent object. |

### isAutoSize {#isAutoSize--}

True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

```javascript
isAutoSize : boolean;
```


### isLink {#isLink--}

Returns true if the OleObject links to the file.

```javascript
isLink : boolean;
```


### displayAsIcon {#displayAsIcon--}

True if the specified object is displayed as an icon and the image will not be auto changed.

```javascript
displayAsIcon : boolean;
```


### imageData {#imageData--}

Represents image of ole object as byte array.

```javascript
imageData : Uint8Array;
```


### objectData {#objectData--}

Represents embedded ole object data as byte array.

```javascript
objectData : Uint8Array;
```


### fullObjectBin {#fullObjectBin--}

Readonly. Gets the full embedded ole object binary data in the template file.

```javascript
fullObjectBin : Uint8Array;
```


### imageSourceFullName {#imageSourceFullName--}

Gets or sets the path and name of the source file for the linked image.

```javascript
imageSourceFullName : string;
```


**Remarks**

The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

### progID {#progID--}

Gets or sets the ProgID of the OLE object.

```javascript
progID : string;
```


### fileFormatType {#fileFormatType--}

Gets and sets the file type of the embedded ole object data

```javascript
fileFormatType : FileFormatType;
```


### objectSourceFullName {#objectSourceFullName--}

Returns the source full name of the source file for the linked OLE object.

```javascript
objectSourceFullName : string;
```


**Remarks**

Only supports setting the source full name when the file type is OleFileType.Unknown. Such as wav file ,avi file..etc..

### label {#label--}

Gets and sets the display label of the linked ole object.

```javascript
label : string;
```


### autoUpdate {#autoUpdate--}

Specifies whether the link to the OleObject is automatically updated or not.

```javascript
autoUpdate : boolean;
```


### autoLoad {#autoLoad--}

Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened.

```javascript
autoLoad : boolean;
```


### classIdentifier {#classIdentifier--}

Gets and sets the class identifier of the embedded object. It means which application opens the embedded file.

```javascript
classIdentifier : Uint8Array;
```


### imageType {#imageType--}

Readonly. Gets the image format of the ole object.

```javascript
imageType : ImageType;
```


### macroName {#macroName--}

Gets and sets the name of macro.

```javascript
macroName : string;
```


### isEquation {#isEquation--}

Readonly. Indicates whether the shape only contains an equation.

```javascript
isEquation : boolean;
```


### isSmartArt {#isSmartArt--}

Readonly. Indicates whether the shape is a smart art.

```javascript
isSmartArt : boolean;
```


**Remarks**

Only for ooxml file.

### zOrderPosition {#zOrderPosition--}

Returns the position of a shape in the z-order.

```javascript
zOrderPosition : number;
```


### name {#name--}

Gets and sets the name of the shape.

```javascript
name : string;
```


### alternativeText {#alternativeText--}

Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object.

```javascript
alternativeText : string;
```


### title {#title--}

Specifies the title (caption) of the current shape object.

```javascript
title : string;
```


### line {#line--}

Readonly. Gets line style

```javascript
line : LineFormat;
```


### fill {#fill--}

Readonly. Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape.

```javascript
fill : FillFormat;
```


### shadowEffect {#shadowEffect--}

Readonly. Represents a [Drawing.ShadowEffect](../drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape.

```javascript
shadowEffect : ShadowEffect;
```


### reflection {#reflection--}

Readonly. Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape.

```javascript
reflection : ReflectionEffect;
```


### glow {#glow--}

Readonly. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape.

```javascript
glow : GlowEffect;
```


### softEdges {#softEdges--}

Gets and sets the radius of blur to apply to the edges, in unit of points.

```javascript
softEdges : number;
```


### threeDFormat {#threeDFormat--}

Readonly. Gets and sets 3d format of the shape.

```javascript
threeDFormat : ThreeDFormat;
```


### formatPicture {#formatPicture--}

Readonly. Gets and sets the options of the picture format.

```javascript
formatPicture : MsoFormatPicture;
```


### isHidden {#isHidden--}

Indicates whether the object is visible.

```javascript
isHidden : boolean;
```


### isLockAspectRatio {#isLockAspectRatio--}

True means that aspect ratio of the shape is locked.

```javascript
isLockAspectRatio : boolean;
```


**Remarks**

Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### isAspectRatioLocked {#isAspectRatioLocked--}

True means that aspect ratio of the shape is locked.

```javascript
isAspectRatioLocked : boolean;
```


**Remarks**

Only for pictures and Ole Objects.

### rotationAngle {#rotationAngle--}

Gets and sets the rotation of the shape.

```javascript
rotationAngle : number;
```


### hyperlink {#hyperlink--}

Readonly. Gets the hyperlink of the shape.

```javascript
hyperlink : Hyperlink;
```


### id {#id--}

Readonly. Gets the identifier of this shape.

```javascript
id : number;
```


### spid {#spid--}

Readonly. Specifies an optional string identifier that an application can use to identify the particular shape.

```javascript
spid : string;
```


### spt {#spt--}

Readonly. Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

```javascript
spt : number;
```


### worksheet {#worksheet--}

Readonly. Gets the [Worksheet](../worksheet/) object which contains this shape.

```javascript
worksheet : Worksheet;
```


### isGroup {#isGroup--}

Readonly. Indicates whether this shape is a group shape.

```javascript
isGroup : boolean;
```


### isInGroup {#isInGroup--}

Readonly. Indicates whether the shape is grouped.

```javascript
isInGroup : boolean;
```


### isWordArt {#isWordArt--}

Readonly. Indicates whether this shape is a word art.

```javascript
isWordArt : boolean;
```


**Remarks**

Only for the Legacy Shape of xls file.

### textEffect {#textEffect--}

Readonly. Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

```javascript
textEffect : TextEffectFormat;
```


### isLocked {#isLocked--}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```javascript
isLocked : boolean;
```


### isPrintable {#isPrintable--}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

```javascript
isPrintable : boolean;
```


### msoDrawingType {#msoDrawingType--}

Readonly. Gets drawing type.

```javascript
msoDrawingType : MsoDrawingType;
```


### autoShapeType {#autoShapeType--}

Gets and sets the auto shape type.

```javascript
autoShapeType : AutoShapeType;
```


### anchorType {#anchorType--}

Gets and set the type of the shape anchor placeholder.

```javascript
anchorType : ShapeAnchorType;
```


### placement {#placement--}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
placement : PlacementType;
```


### upperLeftRow {#upperLeftRow--}

Represents the top row index.

```javascript
upperLeftRow : number;
```


**Remarks**

If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### upperDeltaY {#upperDeltaY--}

Gets or sets the shape's vertical offset from its upper left corner row.

```javascript
upperDeltaY : number;
```


**Remarks**

The range of value is 0 to 256.

### upperLeftColumn {#upperLeftColumn--}

Represents upper left corner column index.

```javascript
upperLeftColumn : number;
```


### upperDeltaX {#upperDeltaX--}

Gets or sets the shape's horizontal offset from its upper left corner column.

```javascript
upperDeltaX : number;
```


**Remarks**

The range of value is 0 to 1024.

### lowerRightRow {#lowerRightRow--}

Represents lower right corner row index.

```javascript
lowerRightRow : number;
```


### lowerDeltaY {#lowerDeltaY--}

Gets or sets the shape's vertical offset from its lower right corner row.

```javascript
lowerDeltaY : number;
```


**Remarks**

The range of value is 0 to 256.

### lowerRightColumn {#lowerRightColumn--}

Represents lower right corner column index.

```javascript
lowerRightColumn : number;
```


### lowerDeltaX {#lowerDeltaX--}

Gets or sets the shape's horizontal  offset from its lower right corner column.

```javascript
lowerDeltaX : number;
```


**Remarks**

The range of value is 0 to 1024.

### right {#right--}

Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels.

```javascript
right : number;
```


### bottom {#bottom--}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

```javascript
bottom : number;
```


### width {#width--}

Represents the width of shape, in unit of pixels.

```javascript
width : number;
```


### widthInch {#widthInch--}

Represents the width of the shape, in unit of inch.

```javascript
widthInch : number;
```


### widthPt {#widthPt--}

Represents the width of the shape, in unit of point.

```javascript
widthPt : number;
```


### widthCM {#widthCM--}

Represents the width of the shape, in unit of centimeters.

```javascript
widthCM : number;
```


### height {#height--}

Represents the height of shape, in unit of pixel.

```javascript
height : number;
```


### heightInch {#heightInch--}

Represents the height of the shape, in unit of inches.

```javascript
heightInch : number;
```


### heightPt {#heightPt--}

Represents the height of the shape, in unit of points.

```javascript
heightPt : number;
```


### heightCM {#heightCM--}

Represents the height of the shape, in unit of centimeters.

```javascript
heightCM : number;
```


### left {#left--}

Represents the horizontal offset of shape from its left column, in unit of pixels.

```javascript
left : number;
```


### leftInch {#leftInch--}

Represents the horizontal offset of shape from its left column, in unit of inches.

```javascript
leftInch : number;
```


### leftCM {#leftCM--}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

```javascript
leftCM : number;
```


### top {#top--}

Represents the vertical offset of shape from its top row, in unit of pixels.

```javascript
top : number;
```


**Remarks**

If the shape is in the chart, represents the vertical offset of shape from its top border.

### topInch {#topInch--}

Represents the vertical offset of shape from its top row, in unit of inches.

```javascript
topInch : number;
```


### topCM {#topCM--}

Represents the vertical offset of shape from its top row, in unit of centimeters.

```javascript
topCM : number;
```


### topToCorner {#topToCorner--}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

```javascript
topToCorner : number;
```


### leftToCorner {#leftToCorner--}

Gets and sets the horizonal offset of shape from worksheet left border.

```javascript
leftToCorner : number;
```


### x {#x--}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

```javascript
x : number;
```


### y {#y--}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

```javascript
y : number;
```


### widthScale {#widthScale--}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

```javascript
widthScale : number;
```


### heightScale {#heightScale--}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

```javascript
heightScale : number;
```


### topInShape {#topInShape--}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.

```javascript
topInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### leftInShape {#leftInShape--}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.

```javascript
leftInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### widthInShape {#widthInShape--}

Represents the width of the shape, in unit of 1/4000 of the parent shape.

```javascript
widthInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### heightInShape {#heightInShape--}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..

```javascript
heightInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### group {#group--}

Readonly. Gets the group shape which contains this shape.

```javascript
group : GroupShape;
```


### type {#type--}

Readonly. Gets the auto shape type.

```javascript
type : AutoShapeType;
```


### hasLine {#hasLine--}

Gets and sets the line border of the shape is visible.

```javascript
hasLine : boolean;
```


### isFilled {#isFilled--}

Indicates whether the fill format is visible.

```javascript
isFilled : boolean;
```


### isFlippedHorizontally {#isFlippedHorizontally--}

Gets and sets whether shape is horizontally flipped .

```javascript
isFlippedHorizontally : boolean;
```


### isFlippedVertically {#isFlippedVertically--}

Gets and sets whether shape is vertically flipped .

```javascript
isFlippedVertically : boolean;
```


### actualLowerRightRow {#actualLowerRightRow--}

Readonly. Get the actual bottom row.

```javascript
actualLowerRightRow : number;
```


### relativeToOriginalPictureSize {#relativeToOriginalPictureSize--}

Indicates whether shape is relative to original picture size.

```javascript
relativeToOriginalPictureSize : boolean;
```


### linkedCell {#linkedCell--}

Gets or sets the worksheet range linked to the control's value.

```javascript
linkedCell : string;
```


### inputRange {#inputRange--}

Gets or sets the worksheet range used to fill the specified combo box.

```javascript
inputRange : string;
```


### textShapeType {#textShapeType--}

Gets and sets the preset text shape type.

```javascript
textShapeType : AutoShapeType;
```


### textBody {#textBody--}

Readonly. Gets and sets the setting of the shape's text.

```javascript
textBody : FontSettingCollection;
```


### font {#font--}

Represents the font of shape.

```javascript
font : Font;
```


### textOptions {#textOptions--}

Represents the text options of the shape.

```javascript
textOptions : TextOptions;
```


### text {#text--}

Gets and sets the text of this shape.

```javascript
text : string;
```


### isRichText {#isRichText--}

Readonly. Whether or not the text is rich text.

```javascript
isRichText : boolean;
```


### htmlText {#htmlText--}

Gets and sets the html string which contains data and some formats in this textbox.

```javascript
htmlText : string;
```


### textVerticalOverflow {#textVerticalOverflow--}

Gets and sets the text vertical overflow type of the shape which contains text.

```javascript
textVerticalOverflow : TextOverflowType;
```


### textHorizontalOverflow {#textHorizontalOverflow--}

Gets and sets the text horizontal overflow type of the shape which contains text.

```javascript
textHorizontalOverflow : TextOverflowType;
```


### isTextWrapped {#isTextWrapped--}

Gets and sets the text wrapped type of the shape which contains text.

```javascript
isTextWrapped : boolean;
```


### textOrientationType {#textOrientationType--}

Gets and sets the text orientation type of the shape.

```javascript
textOrientationType : TextOrientationType;
```


### textHorizontalAlignment {#textHorizontalAlignment--}

Gets and sets the text horizontal alignment type of the shape.

```javascript
textHorizontalAlignment : TextAlignmentType;
```


### textVerticalAlignment {#textVerticalAlignment--}

Gets and sets the text vertical alignment type of the shape.

```javascript
textVerticalAlignment : TextAlignmentType;
```


### textDirection {#textDirection--}

Gets/Sets the direction of the text flow for this object.

```javascript
textDirection : TextDirectionType;
```


### textBoxOptions {#textBoxOptions--}

Readonly. Gets the text information in the shape

```javascript
textBoxOptions : TextBoxOptions;
```


### controlData {#controlData--}

Readonly. Gets the data of control.

```javascript
controlData : Uint8Array;
```


### activeXControl {#activeXControl--}

Readonly. Gets the ActiveX control.

```javascript
activeXControl : ActiveXControl;
```


### paths {#paths--}

Readonly. Gets the paths of a custom geometric shape.

```javascript
paths : ShapePathCollection;
```


### geometry {#geometry--}

Readonly. Gets the geometry

```javascript
geometry : Geometry;
```


### isDecorative {#isDecorative--}

Indicates whether the object is decorative.

```javascript
isDecorative : boolean;
```


### isAutoSize() {#isAutoSize--}

<b>@deprecated.</b> Please use the 'isAutoSize' property instead. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

```javascript
isAutoSize() : boolean;
```


### setIsAutoSize(boolean) {#setIsAutoSize-boolean-}

<b>@deprecated.</b> Please use the 'isAutoSize' property instead. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

```javascript
setIsAutoSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isLink() {#isLink--}

<b>@deprecated.</b> Please use the 'isLink' property instead. Returns true if the OleObject links to the file.

```javascript
isLink() : boolean;
```


### set_IsLink(boolean) {#set_IsLink-boolean-}

<b>@deprecated.</b> Please use the 'isLink' property instead. Returns true if the OleObject links to the file.

```javascript
set_IsLink(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayAsIcon() {#getDisplayAsIcon--}

<b>@deprecated.</b> Please use the 'displayAsIcon' property instead. True if the specified object is displayed as an icon and the image will not be auto changed.

```javascript
getDisplayAsIcon() : boolean;
```


### setDisplayAsIcon(boolean) {#setDisplayAsIcon-boolean-}

<b>@deprecated.</b> Please use the 'displayAsIcon' property instead. True if the specified object is displayed as an icon and the image will not be auto changed.

```javascript
setDisplayAsIcon(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getImageData() {#getImageData--}

<b>@deprecated.</b> Please use the 'imageData' property instead. Represents image of ole object as byte array.

```javascript
getImageData() : Uint8Array;
```


### setImageData(Uint8Array) {#setImageData-uint8array-}

<b>@deprecated.</b> Please use the 'imageData' property instead. Represents image of ole object as byte array.

```javascript
setImageData(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getObjectData() {#getObjectData--}

<b>@deprecated.</b> Please use the 'objectData' property instead. Represents embedded ole object data as byte array.

```javascript
getObjectData() : Uint8Array;
```


### setObjectData(Uint8Array) {#setObjectData-uint8array-}

<b>@deprecated.</b> Please use the 'objectData' property instead. Represents embedded ole object data as byte array.

```javascript
setObjectData(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getFullObjectBin() {#getFullObjectBin--}

<b>@deprecated.</b> Please use the 'fullObjectBin' property instead. Gets the full embedded ole object binary data in the template file.

```javascript
getFullObjectBin() : Uint8Array;
```


### getImageSourceFullName() {#getImageSourceFullName--}

<b>@deprecated.</b> Please use the 'imageSourceFullName' property instead. Gets or sets the path and name of the source file for the linked image.

```javascript
getImageSourceFullName() : string;
```


**Remarks**

The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

### setImageSourceFullName(string) {#setImageSourceFullName-string-}

<b>@deprecated.</b> Please use the 'imageSourceFullName' property instead. Gets or sets the path and name of the source file for the linked image.

```javascript
setImageSourceFullName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

### getProgID() {#getProgID--}

<b>@deprecated.</b> Please use the 'progID' property instead. Gets or sets the ProgID of the OLE object.

```javascript
getProgID() : string;
```


### setProgID(string) {#setProgID-string-}

<b>@deprecated.</b> Please use the 'progID' property instead. Gets or sets the ProgID of the OLE object.

```javascript
setProgID(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getFileFormatType() {#getFileFormatType--}

<b>@deprecated.</b> Please use the 'fileFormatType' property instead. Gets and sets the file type of the embedded ole object data

```javascript
getFileFormatType() : FileFormatType;
```


**Returns**

[FileFormatType](../fileformattype/)

### setFileFormatType(FileFormatType) {#setFileFormatType-fileformattype-}

<b>@deprecated.</b> Please use the 'fileFormatType' property instead. Gets and sets the file type of the embedded ole object data

```javascript
setFileFormatType(value: FileFormatType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FileFormatType](../fileformattype/) | The value to set. |

### getObjectSourceFullName() {#getObjectSourceFullName--}

<b>@deprecated.</b> Please use the 'objectSourceFullName' property instead. Returns the source full name of the source file for the linked OLE object.

```javascript
getObjectSourceFullName() : string;
```


**Remarks**

Only supports setting the source full name when the file type is OleFileType.Unknown. Such as wav file ,avi file..etc..

### setObjectSourceFullName(string) {#setObjectSourceFullName-string-}

<b>@deprecated.</b> Please use the 'objectSourceFullName' property instead. Returns the source full name of the source file for the linked OLE object.

```javascript
setObjectSourceFullName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

Only supports setting the source full name when the file type is OleFileType.Unknown. Such as wav file ,avi file..etc..

### getLabel() {#getLabel--}

<b>@deprecated.</b> Please use the 'label' property instead. Gets and sets the display label of the linked ole object.

```javascript
getLabel() : string;
```


### setLabel(string) {#setLabel-string-}

<b>@deprecated.</b> Please use the 'label' property instead. Gets and sets the display label of the linked ole object.

```javascript
setLabel(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAutoUpdate() {#getAutoUpdate--}

<b>@deprecated.</b> Please use the 'autoUpdate' property instead. Specifies whether the link to the OleObject is automatically updated or not.

```javascript
getAutoUpdate() : boolean;
```


### setAutoUpdate(boolean) {#setAutoUpdate-boolean-}

<b>@deprecated.</b> Please use the 'autoUpdate' property instead. Specifies whether the link to the OleObject is automatically updated or not.

```javascript
setAutoUpdate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoLoad() {#getAutoLoad--}

<b>@deprecated.</b> Please use the 'autoLoad' property instead. Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened.

```javascript
getAutoLoad() : boolean;
```


### setAutoLoad(boolean) {#setAutoLoad-boolean-}

<b>@deprecated.</b> Please use the 'autoLoad' property instead. Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened.

```javascript
setAutoLoad(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getClassIdentifier() {#getClassIdentifier--}

<b>@deprecated.</b> Please use the 'classIdentifier' property instead. Gets and sets the class identifier of the embedded object. It means which application opens the embedded file.

```javascript
getClassIdentifier() : Uint8Array;
```


### setClassIdentifier(Uint8Array) {#setClassIdentifier-uint8array-}

<b>@deprecated.</b> Please use the 'classIdentifier' property instead. Gets and sets the class identifier of the embedded object. It means which application opens the embedded file.

```javascript
setClassIdentifier(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getImageType() {#getImageType--}

<b>@deprecated.</b> Please use the 'imageType' property instead. Gets the image format of the ole object.

```javascript
getImageType() : ImageType;
```


**Returns**

[ImageType](../imagetype/)

### setEmbeddedObject(boolean, Uint8Array, string, boolean, string) {#setEmbeddedObject-boolean-uint8array-string-boolean-string-}

Sets embedded object data.

```javascript
setEmbeddedObject(linkToFile: boolean, objectData: Uint8Array, sourceFileName: string, displayAsIcon: boolean, label: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | number[] | The embedded object data. |
| sourceFileName | string | The file name. |
| displayAsIcon | boolean | Indicates whether diplaying object as an icon.         /// If true, the orginal image data will be covered by icon. |
| label | string | The icon label. Only works when displayAsIcon as true. |

### setEmbeddedObject(boolean, Uint8Array, string, boolean, string, boolean) {#setEmbeddedObject-boolean-uint8array-string-boolean-string-boolean-}

Sets embedded object data.

```javascript
setEmbeddedObject(linkToFile: boolean, objectData: Uint8Array, sourceFileName: string, displayAsIcon: boolean, label: string, updateIcon: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | number[] | The embedded object data. |
| sourceFileName | string | The file name. |
| displayAsIcon | boolean | Indicates whether diplaying object as an icon.         /// If true, the orginal image data will be covered by icon. |
| label | string | The icon label. Only works when displayAsIcon as true. |
| updateIcon | boolean | Indicates whether automatically updating icon. |

**Remarks**

As Aspose can update embedd all file icons, so it's better that you can add correct icon with <paramref name="updateIcon"/> as false.

### setNativeSourceFullName(string) {#setNativeSourceFullName-string-}

Sets the ole native source full file name with path.

```javascript
setNativeSourceFullName(sourceFullName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceFullName | string | the ole native source full file name |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getMacroName() {#getMacroName--}

<b>@deprecated.</b> Please use the 'macroName' property instead. Gets and sets the name of macro.

```javascript
getMacroName() : string;
```


### setMacroName(string) {#setMacroName-string-}

<b>@deprecated.</b> Please use the 'macroName' property instead. Gets and sets the name of macro.

```javascript
setMacroName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isEquation() {#isEquation--}

<b>@deprecated.</b> Please use the 'isEquation' property instead. Indicates whether the shape only contains an equation.

```javascript
isEquation() : boolean;
```


### isSmartArt() {#isSmartArt--}

<b>@deprecated.</b> Please use the 'isSmartArt' property instead. Indicates whether the shape is a smart art.

```javascript
isSmartArt() : boolean;
```


**Remarks**

Only for ooxml file.

### getZOrderPosition() {#getZOrderPosition--}

<b>@deprecated.</b> Please use the 'zOrderPosition' property instead. Returns the position of a shape in the z-order.

```javascript
getZOrderPosition() : number;
```


### setZOrderPosition(number) {#setZOrderPosition-number-}

<b>@deprecated.</b> Please use the 'zOrderPosition' property instead. Returns the position of a shape in the z-order.

```javascript
setZOrderPosition(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getName() {#getName--}

<b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the shape.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

<b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the shape.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAlternativeText() {#getAlternativeText--}

<b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object.

```javascript
getAlternativeText() : string;
```


### setAlternativeText(string) {#setAlternativeText-string-}

<b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object.

```javascript
setAlternativeText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTitle() {#getTitle--}

<b>@deprecated.</b> Please use the 'title' property instead. Specifies the title (caption) of the current shape object.

```javascript
getTitle() : string;
```


### setTitle(string) {#setTitle-string-}

<b>@deprecated.</b> Please use the 'title' property instead. Specifies the title (caption) of the current shape object.

```javascript
setTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getLine() {#getLine--}

<b>@deprecated.</b> Please use the 'line' property instead. Gets line style

```javascript
getLine() : LineFormat;
```


**Returns**

[LineFormat](../lineformat/)

### getFill() {#getFill--}

<b>@deprecated.</b> Please use the 'fill' property instead. Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape.

```javascript
getFill() : FillFormat;
```


**Returns**

[FillFormat](../fillformat/)

### getShadowEffect() {#getShadowEffect--}

<b>@deprecated.</b> Please use the 'shadowEffect' property instead. Represents a [Drawing.ShadowEffect](../drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape.

```javascript
getShadowEffect() : ShadowEffect;
```


**Returns**

[ShadowEffect](../shadoweffect/)

### getReflection() {#getReflection--}

<b>@deprecated.</b> Please use the 'reflection' property instead. Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape.

```javascript
getReflection() : ReflectionEffect;
```


**Returns**

[ReflectionEffect](../reflectioneffect/)

### getGlow() {#getGlow--}

<b>@deprecated.</b> Please use the 'glow' property instead. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape.

```javascript
getGlow() : GlowEffect;
```


**Returns**

[GlowEffect](../gloweffect/)

### getSoftEdges() {#getSoftEdges--}

<b>@deprecated.</b> Please use the 'softEdges' property instead. Gets and sets the radius of blur to apply to the edges, in unit of points.

```javascript
getSoftEdges() : number;
```


### setSoftEdges(number) {#setSoftEdges-number-}

<b>@deprecated.</b> Please use the 'softEdges' property instead. Gets and sets the radius of blur to apply to the edges, in unit of points.

```javascript
setSoftEdges(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getThreeDFormat() {#getThreeDFormat--}

<b>@deprecated.</b> Please use the 'threeDFormat' property instead. Gets and sets 3d format of the shape.

```javascript
getThreeDFormat() : ThreeDFormat;
```


**Returns**

[ThreeDFormat](../threedformat/)

### getFormatPicture() {#getFormatPicture--}

<b>@deprecated.</b> Please use the 'formatPicture' property instead. Gets and sets the options of the picture format.

```javascript
getFormatPicture() : MsoFormatPicture;
```


**Returns**

[MsoFormatPicture](../msoformatpicture/)

### isHidden() {#isHidden--}

<b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether the object is visible.

```javascript
isHidden() : boolean;
```


### setIsHidden(boolean) {#setIsHidden-boolean-}

<b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether the object is visible.

```javascript
setIsHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isLockAspectRatio() {#isLockAspectRatio--}

<b>@deprecated.</b> Please use the 'isLockAspectRatio' property instead. True means that aspect ratio of the shape is locked.

```javascript
isLockAspectRatio() : boolean;
```


**Remarks**

Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### setIsLockAspectRatio(boolean) {#setIsLockAspectRatio-boolean-}

<b>@deprecated.</b> Please use the 'isLockAspectRatio' property instead. True means that aspect ratio of the shape is locked.

```javascript
setIsLockAspectRatio(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### isAspectRatioLocked() {#isAspectRatioLocked--}

<b>@deprecated.</b> Please use the 'isAspectRatioLocked' property instead. True means that aspect ratio of the shape is locked.

```javascript
isAspectRatioLocked() : boolean;
```


**Remarks**

Only for pictures and Ole Objects.

### setIsAspectRatioLocked(boolean) {#setIsAspectRatioLocked-boolean-}

<b>@deprecated.</b> Please use the 'isAspectRatioLocked' property instead. True means that aspect ratio of the shape is locked.

```javascript
setIsAspectRatioLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for pictures and Ole Objects.

### getRotationAngle() {#getRotationAngle--}

<b>@deprecated.</b> Please use the 'rotationAngle' property instead. Gets and sets the rotation of the shape.

```javascript
getRotationAngle() : number;
```


### setRotationAngle(number) {#setRotationAngle-number-}

<b>@deprecated.</b> Please use the 'rotationAngle' property instead. Gets and sets the rotation of the shape.

```javascript
setRotationAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHyperlink() {#getHyperlink--}

<b>@deprecated.</b> Please use the 'hyperlink' property instead. Gets the hyperlink of the shape.

```javascript
getHyperlink() : Hyperlink;
```


**Returns**

[Hyperlink](../hyperlink/)

### getId() {#getId--}

<b>@deprecated.</b> Please use the 'id' property instead. Gets the identifier of this shape.

```javascript
getId() : number;
```


### getSpid() {#getSpid--}

<b>@deprecated.</b> Please use the 'spid' property instead. Specifies an optional string identifier that an application can use to identify the particular shape.

```javascript
getSpid() : string;
```


### getSpt() {#getSpt--}

<b>@deprecated.</b> Please use the 'spt' property instead. Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

```javascript
getSpt() : number;
```


### getWorksheet() {#getWorksheet--}

<b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the [Worksheet](../worksheet/) object which contains this shape.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

### isGroup() {#isGroup--}

<b>@deprecated.</b> Please use the 'isGroup' property instead. Indicates whether this shape is a group shape.

```javascript
isGroup() : boolean;
```


### isInGroup() {#isInGroup--}

<b>@deprecated.</b> Please use the 'isInGroup' property instead. Indicates whether the shape is grouped.

```javascript
isInGroup() : boolean;
```


### isWordArt() {#isWordArt--}

<b>@deprecated.</b> Please use the 'isWordArt' property instead. Indicates whether this shape is a word art.

```javascript
isWordArt() : boolean;
```


**Remarks**

Only for the Legacy Shape of xls file.

### getTextEffect() {#getTextEffect--}

<b>@deprecated.</b> Please use the 'textEffect' property instead. Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

```javascript
getTextEffect() : TextEffectFormat;
```


**Returns**

[TextEffectFormat](../texteffectformat/)

### isLocked() {#isLocked--}

<b>@deprecated.</b> Please use the 'isLocked' property instead. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```javascript
isLocked() : boolean;
```


### setIsLocked(boolean) {#setIsLocked-boolean-}

<b>@deprecated.</b> Please use the 'isLocked' property instead. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isPrintable() {#isPrintable--}

<b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the object is printable. If False, this shape will not be printed when printing.

```javascript
isPrintable() : boolean;
```


### setIsPrintable(boolean) {#setIsPrintable-boolean-}

<b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the object is printable. If False, this shape will not be printed when printing.

```javascript
setIsPrintable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMsoDrawingType() {#getMsoDrawingType--}

<b>@deprecated.</b> Please use the 'msoDrawingType' property instead. Gets drawing type.

```javascript
getMsoDrawingType() : MsoDrawingType;
```


**Returns**

[MsoDrawingType](../msodrawingtype/)

### getAutoShapeType() {#getAutoShapeType--}

<b>@deprecated.</b> Please use the 'autoShapeType' property instead. Gets and sets the auto shape type.

```javascript
getAutoShapeType() : AutoShapeType;
```


**Returns**

[AutoShapeType](../autoshapetype/)

### setAutoShapeType(AutoShapeType) {#setAutoShapeType-autoshapetype-}

<b>@deprecated.</b> Please use the 'autoShapeType' property instead. Gets and sets the auto shape type.

```javascript
setAutoShapeType(value: AutoShapeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoShapeType](../autoshapetype/) | The value to set. |

### getAnchorType() {#getAnchorType--}

<b>@deprecated.</b> Please use the 'anchorType' property instead. Gets and set the type of the shape anchor placeholder.

```javascript
getAnchorType() : ShapeAnchorType;
```


**Returns**

[ShapeAnchorType](../shapeanchortype/)

### setAnchorType(ShapeAnchorType) {#setAnchorType-shapeanchortype-}

<b>@deprecated.</b> Please use the 'anchorType' property instead. Gets and set the type of the shape anchor placeholder.

```javascript
setAnchorType(value: ShapeAnchorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ShapeAnchorType](../shapeanchortype/) | The value to set. |

### getPlacement() {#getPlacement--}

<b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
getPlacement() : PlacementType;
```


**Returns**

[PlacementType](../placementtype/)

### setPlacement(PlacementType) {#setPlacement-placementtype-}

<b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
setPlacement(value: PlacementType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlacementType](../placementtype/) | The value to set. |

### getUpperLeftRow() {#getUpperLeftRow--}

<b>@deprecated.</b> Please use the 'upperLeftRow' property instead. Represents the top row index.

```javascript
getUpperLeftRow() : number;
```


**Remarks**

If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### setUpperLeftRow(number) {#setUpperLeftRow-number-}

<b>@deprecated.</b> Please use the 'upperLeftRow' property instead. Represents the top row index.

```javascript
setUpperLeftRow(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### getUpperDeltaY() {#getUpperDeltaY--}

<b>@deprecated.</b> Please use the 'upperDeltaY' property instead. Gets or sets the shape's vertical offset from its upper left corner row.

```javascript
getUpperDeltaY() : number;
```


**Remarks**

The range of value is 0 to 256.

### setUpperDeltaY(number) {#setUpperDeltaY-number-}

<b>@deprecated.</b> Please use the 'upperDeltaY' property instead. Gets or sets the shape's vertical offset from its upper left corner row.

```javascript
setUpperDeltaY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 256.

### getUpperLeftColumn() {#getUpperLeftColumn--}

<b>@deprecated.</b> Please use the 'upperLeftColumn' property instead. Represents upper left corner column index.

```javascript
getUpperLeftColumn() : number;
```


### setUpperLeftColumn(number) {#setUpperLeftColumn-number-}

<b>@deprecated.</b> Please use the 'upperLeftColumn' property instead. Represents upper left corner column index.

```javascript
setUpperLeftColumn(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getUpperDeltaX() {#getUpperDeltaX--}

<b>@deprecated.</b> Please use the 'upperDeltaX' property instead. Gets or sets the shape's horizontal offset from its upper left corner column.

```javascript
getUpperDeltaX() : number;
```


**Remarks**

The range of value is 0 to 1024.

### setUpperDeltaX(number) {#setUpperDeltaX-number-}

<b>@deprecated.</b> Please use the 'upperDeltaX' property instead. Gets or sets the shape's horizontal offset from its upper left corner column.

```javascript
setUpperDeltaX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 1024.

### getLowerRightRow() {#getLowerRightRow--}

<b>@deprecated.</b> Please use the 'lowerRightRow' property instead. Represents lower right corner row index.

```javascript
getLowerRightRow() : number;
```


### setLowerRightRow(number) {#setLowerRightRow-number-}

<b>@deprecated.</b> Please use the 'lowerRightRow' property instead. Represents lower right corner row index.

```javascript
setLowerRightRow(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLowerDeltaY() {#getLowerDeltaY--}

<b>@deprecated.</b> Please use the 'lowerDeltaY' property instead. Gets or sets the shape's vertical offset from its lower right corner row.

```javascript
getLowerDeltaY() : number;
```


**Remarks**

The range of value is 0 to 256.

### setLowerDeltaY(number) {#setLowerDeltaY-number-}

<b>@deprecated.</b> Please use the 'lowerDeltaY' property instead. Gets or sets the shape's vertical offset from its lower right corner row.

```javascript
setLowerDeltaY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 256.

### getLowerRightColumn() {#getLowerRightColumn--}

<b>@deprecated.</b> Please use the 'lowerRightColumn' property instead. Represents lower right corner column index.

```javascript
getLowerRightColumn() : number;
```


### setLowerRightColumn(number) {#setLowerRightColumn-number-}

<b>@deprecated.</b> Please use the 'lowerRightColumn' property instead. Represents lower right corner column index.

```javascript
setLowerRightColumn(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLowerDeltaX() {#getLowerDeltaX--}

<b>@deprecated.</b> Please use the 'lowerDeltaX' property instead. Gets or sets the shape's horizontal  offset from its lower right corner column.

```javascript
getLowerDeltaX() : number;
```


**Remarks**

The range of value is 0 to 1024.

### setLowerDeltaX(number) {#setLowerDeltaX-number-}

<b>@deprecated.</b> Please use the 'lowerDeltaX' property instead. Gets or sets the shape's horizontal  offset from its lower right corner column.

```javascript
setLowerDeltaX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 1024.

### getRight() {#getRight--}

<b>@deprecated.</b> Please use the 'right' property instead. Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels.

```javascript
getRight() : number;
```


### setRight(number) {#setRight-number-}

<b>@deprecated.</b> Please use the 'right' property instead. Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels.

```javascript
setRight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBottom() {#getBottom--}

<b>@deprecated.</b> Please use the 'bottom' property instead. Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

```javascript
getBottom() : number;
```


### setBottom(number) {#setBottom-number-}

<b>@deprecated.</b> Please use the 'bottom' property instead. Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

```javascript
setBottom(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidth() {#getWidth--}

<b>@deprecated.</b> Please use the 'width' property instead. Represents the width of shape, in unit of pixels.

```javascript
getWidth() : number;
```


### setWidth(number) {#setWidth-number-}

<b>@deprecated.</b> Please use the 'width' property instead. Represents the width of shape, in unit of pixels.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthInch() {#getWidthInch--}

<b>@deprecated.</b> Please use the 'widthInch' property instead. Represents the width of the shape, in unit of inch.

```javascript
getWidthInch() : number;
```


### setWidthInch(number) {#setWidthInch-number-}

<b>@deprecated.</b> Please use the 'widthInch' property instead. Represents the width of the shape, in unit of inch.

```javascript
setWidthInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthPt() {#getWidthPt--}

<b>@deprecated.</b> Please use the 'widthPt' property instead. Represents the width of the shape, in unit of point.

```javascript
getWidthPt() : number;
```


### setWidthPt(number) {#setWidthPt-number-}

<b>@deprecated.</b> Please use the 'widthPt' property instead. Represents the width of the shape, in unit of point.

```javascript
setWidthPt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthCM() {#getWidthCM--}

<b>@deprecated.</b> Please use the 'widthCM' property instead. Represents the width of the shape, in unit of centimeters.

```javascript
getWidthCM() : number;
```


### setWidthCM(number) {#setWidthCM-number-}

<b>@deprecated.</b> Please use the 'widthCM' property instead. Represents the width of the shape, in unit of centimeters.

```javascript
setWidthCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeight() {#getHeight--}

<b>@deprecated.</b> Please use the 'height' property instead. Represents the height of shape, in unit of pixel.

```javascript
getHeight() : number;
```


### setHeight(number) {#setHeight-number-}

<b>@deprecated.</b> Please use the 'height' property instead. Represents the height of shape, in unit of pixel.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightInch() {#getHeightInch--}

<b>@deprecated.</b> Please use the 'heightInch' property instead. Represents the height of the shape, in unit of inches.

```javascript
getHeightInch() : number;
```


### setHeightInch(number) {#setHeightInch-number-}

<b>@deprecated.</b> Please use the 'heightInch' property instead. Represents the height of the shape, in unit of inches.

```javascript
setHeightInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightPt() {#getHeightPt--}

<b>@deprecated.</b> Please use the 'heightPt' property instead. Represents the height of the shape, in unit of points.

```javascript
getHeightPt() : number;
```


### setHeightPt(number) {#setHeightPt-number-}

<b>@deprecated.</b> Please use the 'heightPt' property instead. Represents the height of the shape, in unit of points.

```javascript
setHeightPt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightCM() {#getHeightCM--}

<b>@deprecated.</b> Please use the 'heightCM' property instead. Represents the height of the shape, in unit of centimeters.

```javascript
getHeightCM() : number;
```


### setHeightCM(number) {#setHeightCM-number-}

<b>@deprecated.</b> Please use the 'heightCM' property instead. Represents the height of the shape, in unit of centimeters.

```javascript
setHeightCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeft() {#getLeft--}

<b>@deprecated.</b> Please use the 'left' property instead. Represents the horizontal offset of shape from its left column, in unit of pixels.

```javascript
getLeft() : number;
```


### setLeft(number) {#setLeft-number-}

<b>@deprecated.</b> Please use the 'left' property instead. Represents the horizontal offset of shape from its left column, in unit of pixels.

```javascript
setLeft(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftInch() {#getLeftInch--}

<b>@deprecated.</b> Please use the 'leftInch' property instead. Represents the horizontal offset of shape from its left column, in unit of inches.

```javascript
getLeftInch() : number;
```


### setLeftInch(number) {#setLeftInch-number-}

<b>@deprecated.</b> Please use the 'leftInch' property instead. Represents the horizontal offset of shape from its left column, in unit of inches.

```javascript
setLeftInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftCM() {#getLeftCM--}

<b>@deprecated.</b> Please use the 'leftCM' property instead. Represents the horizontal offset of shape from its left column, in unit of centimeters.

```javascript
getLeftCM() : number;
```


### setLeftCM(number) {#setLeftCM-number-}

<b>@deprecated.</b> Please use the 'leftCM' property instead. Represents the horizontal offset of shape from its left column, in unit of centimeters.

```javascript
setLeftCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTop() {#getTop--}

<b>@deprecated.</b> Please use the 'top' property instead. Represents the vertical offset of shape from its top row, in unit of pixels.

```javascript
getTop() : number;
```


**Remarks**

If the shape is in the chart, represents the vertical offset of shape from its top border.

### setTop(number) {#setTop-number-}

<b>@deprecated.</b> Please use the 'top' property instead. Represents the vertical offset of shape from its top row, in unit of pixels.

```javascript
setTop(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If the shape is in the chart, represents the vertical offset of shape from its top border.

### getTopInch() {#getTopInch--}

<b>@deprecated.</b> Please use the 'topInch' property instead. Represents the vertical offset of shape from its top row, in unit of inches.

```javascript
getTopInch() : number;
```


### setTopInch(number) {#setTopInch-number-}

<b>@deprecated.</b> Please use the 'topInch' property instead. Represents the vertical offset of shape from its top row, in unit of inches.

```javascript
setTopInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopCM() {#getTopCM--}

<b>@deprecated.</b> Please use the 'topCM' property instead. Represents the vertical offset of shape from its top row, in unit of centimeters.

```javascript
getTopCM() : number;
```


### setTopCM(number) {#setTopCM-number-}

<b>@deprecated.</b> Please use the 'topCM' property instead. Represents the vertical offset of shape from its top row, in unit of centimeters.

```javascript
setTopCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopToCorner() {#getTopToCorner--}

<b>@deprecated.</b> Please use the 'topToCorner' property instead. Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

```javascript
getTopToCorner() : number;
```


### setTopToCorner(number) {#setTopToCorner-number-}

<b>@deprecated.</b> Please use the 'topToCorner' property instead. Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

```javascript
setTopToCorner(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftToCorner() {#getLeftToCorner--}

<b>@deprecated.</b> Please use the 'leftToCorner' property instead. Gets and sets the horizonal offset of shape from worksheet left border.

```javascript
getLeftToCorner() : number;
```


### setLeftToCorner(number) {#setLeftToCorner-number-}

<b>@deprecated.</b> Please use the 'leftToCorner' property instead. Gets and sets the horizonal offset of shape from worksheet left border.

```javascript
setLeftToCorner(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getX() {#getX--}

<b>@deprecated.</b> Please use the 'x' property instead. Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

```javascript
getX() : number;
```


### setX(number) {#setX-number-}

<b>@deprecated.</b> Please use the 'x' property instead. Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

```javascript
setX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getY() {#getY--}

<b>@deprecated.</b> Please use the 'y' property instead. Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

```javascript
getY() : number;
```


### setY(number) {#setY-number-}

<b>@deprecated.</b> Please use the 'y' property instead. Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

```javascript
setY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthScale() {#getWidthScale--}

<b>@deprecated.</b> Please use the 'widthScale' property instead. Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

```javascript
getWidthScale() : number;
```


### setWidthScale(number) {#setWidthScale-number-}

<b>@deprecated.</b> Please use the 'widthScale' property instead. Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

```javascript
setWidthScale(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightScale() {#getHeightScale--}

<b>@deprecated.</b> Please use the 'heightScale' property instead. Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

```javascript
getHeightScale() : number;
```


### setHeightScale(number) {#setHeightScale-number-}

<b>@deprecated.</b> Please use the 'heightScale' property instead. Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

```javascript
setHeightScale(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopInShape() {#getTopInShape--}

<b>@deprecated.</b> Please use the 'topInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.

```javascript
getTopInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setTopInShape(number) {#setTopInShape-number-}

<b>@deprecated.</b> Please use the 'topInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.

```javascript
setTopInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getLeftInShape() {#getLeftInShape--}

<b>@deprecated.</b> Please use the 'leftInShape' property instead. Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.

```javascript
getLeftInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setLeftInShape(number) {#setLeftInShape-number-}

<b>@deprecated.</b> Please use the 'leftInShape' property instead. Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.

```javascript
setLeftInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getWidthInShape() {#getWidthInShape--}

<b>@deprecated.</b> Please use the 'widthInShape' property instead. Represents the width of the shape, in unit of 1/4000 of the parent shape.

```javascript
getWidthInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setWidthInShape(number) {#setWidthInShape-number-}

<b>@deprecated.</b> Please use the 'widthInShape' property instead. Represents the width of the shape, in unit of 1/4000 of the parent shape.

```javascript
setWidthInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getHeightInShape() {#getHeightInShape--}

<b>@deprecated.</b> Please use the 'heightInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..

```javascript
getHeightInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setHeightInShape(number) {#setHeightInShape-number-}

<b>@deprecated.</b> Please use the 'heightInShape' property instead. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..

```javascript
setHeightInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getGroup() {#getGroup--}

<b>@deprecated.</b> Please use the 'group' property instead. Gets the group shape which contains this shape.

```javascript
getGroup() : GroupShape;
```


**Returns**

[GroupShape](../groupshape/)

### getType() {#getType--}

<b>@deprecated.</b> Please use the 'type' property instead. Gets the auto shape type.

```javascript
getType() : AutoShapeType;
```


**Returns**

[AutoShapeType](../autoshapetype/)

### getHasLine() {#getHasLine--}

<b>@deprecated.</b> Please use the 'hasLine' property instead. Gets and sets the line border of the shape is visible.

```javascript
getHasLine() : boolean;
```


### setHasLine(boolean) {#setHasLine-boolean-}

<b>@deprecated.</b> Please use the 'hasLine' property instead. Gets and sets the line border of the shape is visible.

```javascript
setHasLine(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFilled() {#isFilled--}

<b>@deprecated.</b> Please use the 'isFilled' property instead. Indicates whether the fill format is visible.

```javascript
isFilled() : boolean;
```


### setIsFilled(boolean) {#setIsFilled-boolean-}

<b>@deprecated.</b> Please use the 'isFilled' property instead. Indicates whether the fill format is visible.

```javascript
setIsFilled(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFlippedHorizontally() {#isFlippedHorizontally--}

<b>@deprecated.</b> Please use the 'isFlippedHorizontally' property instead. Gets and sets whether shape is horizontally flipped .

```javascript
isFlippedHorizontally() : boolean;
```


### setIsFlippedHorizontally(boolean) {#setIsFlippedHorizontally-boolean-}

<b>@deprecated.</b> Please use the 'isFlippedHorizontally' property instead. Gets and sets whether shape is horizontally flipped .

```javascript
setIsFlippedHorizontally(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFlippedVertically() {#isFlippedVertically--}

<b>@deprecated.</b> Please use the 'isFlippedVertically' property instead. Gets and sets whether shape is vertically flipped .

```javascript
isFlippedVertically() : boolean;
```


### setIsFlippedVertically(boolean) {#setIsFlippedVertically-boolean-}

<b>@deprecated.</b> Please use the 'isFlippedVertically' property instead. Gets and sets whether shape is vertically flipped .

```javascript
setIsFlippedVertically(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getActualLowerRightRow() {#getActualLowerRightRow--}

<b>@deprecated.</b> Please use the 'actualLowerRightRow' property instead. Get the actual bottom row.

```javascript
getActualLowerRightRow() : number;
```


### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}

<b>@deprecated.</b> Please use the 'relativeToOriginalPictureSize' property instead. Indicates whether shape is relative to original picture size.

```javascript
getRelativeToOriginalPictureSize() : boolean;
```


### setRelativeToOriginalPictureSize(boolean) {#setRelativeToOriginalPictureSize-boolean-}

<b>@deprecated.</b> Please use the 'relativeToOriginalPictureSize' property instead. Indicates whether shape is relative to original picture size.

```javascript
setRelativeToOriginalPictureSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLinkedCell() {#getLinkedCell--}

<b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets or sets the worksheet range linked to the control's value.

```javascript
getLinkedCell() : string;
```


### setLinkedCell(string) {#setLinkedCell-string-}

<b>@deprecated.</b> Please use the 'linkedCell' property instead. Gets or sets the worksheet range linked to the control's value.

```javascript
setLinkedCell(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getInputRange() {#getInputRange--}

<b>@deprecated.</b> Please use the 'inputRange' property instead. Gets or sets the worksheet range used to fill the specified combo box.

```javascript
getInputRange() : string;
```


### setInputRange(string) {#setInputRange-string-}

<b>@deprecated.</b> Please use the 'inputRange' property instead. Gets or sets the worksheet range used to fill the specified combo box.

```javascript
setInputRange(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTextShapeType() {#getTextShapeType--}

<b>@deprecated.</b> Please use the 'textShapeType' property instead. Gets and sets the preset text shape type.

```javascript
getTextShapeType() : AutoShapeType;
```


**Returns**

[AutoShapeType](../autoshapetype/)

### setTextShapeType(AutoShapeType) {#setTextShapeType-autoshapetype-}

<b>@deprecated.</b> Please use the 'textShapeType' property instead. Gets and sets the preset text shape type.

```javascript
setTextShapeType(value: AutoShapeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoShapeType](../autoshapetype/) | The value to set. |

### getTextBody() {#getTextBody--}

<b>@deprecated.</b> Please use the 'textBody' property instead. Gets and sets the setting of the shape's text.

```javascript
getTextBody() : FontSettingCollection;
```


**Returns**

[FontSettingCollection](../fontsettingcollection/)

### getFont() {#getFont--}

<b>@deprecated.</b> Please use the 'font' property instead. Represents the font of shape.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### setFont(Font) {#setFont-font-}

<b>@deprecated.</b> Please use the 'font' property instead. Represents the font of shape.

```javascript
setFont(value: Font) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Font](../font/) | The value to set. |

### getTextOptions() {#getTextOptions--}

<b>@deprecated.</b> Please use the 'textOptions' property instead. Represents the text options of the shape.

```javascript
getTextOptions() : TextOptions;
```


**Returns**

[TextOptions](../textoptions/)

### setTextOptions(TextOptions) {#setTextOptions-textoptions-}

<b>@deprecated.</b> Please use the 'textOptions' property instead. Represents the text options of the shape.

```javascript
setTextOptions(value: TextOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOptions](../textoptions/) | The value to set. |

### getText() {#getText--}

<b>@deprecated.</b> Please use the 'text' property instead. Gets and sets the text of this shape.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

<b>@deprecated.</b> Please use the 'text' property instead. Gets and sets the text of this shape.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isRichText() {#isRichText--}

<b>@deprecated.</b> Please use the 'isRichText' property instead. Whether or not the text is rich text.

```javascript
isRichText() : boolean;
```


### getHtmlText() {#getHtmlText--}

<b>@deprecated.</b> Please use the 'htmlText' property instead. Gets and sets the html string which contains data and some formats in this textbox.

```javascript
getHtmlText() : string;
```


### setHtmlText(string) {#setHtmlText-string-}

<b>@deprecated.</b> Please use the 'htmlText' property instead. Gets and sets the html string which contains data and some formats in this textbox.

```javascript
setHtmlText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTextVerticalOverflow() {#getTextVerticalOverflow--}

<b>@deprecated.</b> Please use the 'textVerticalOverflow' property instead. Gets and sets the text vertical overflow type of the shape which contains text.

```javascript
getTextVerticalOverflow() : TextOverflowType;
```


**Returns**

[TextOverflowType](../textoverflowtype/)

### setTextVerticalOverflow(TextOverflowType) {#setTextVerticalOverflow-textoverflowtype-}

<b>@deprecated.</b> Please use the 'textVerticalOverflow' property instead. Gets and sets the text vertical overflow type of the shape which contains text.

```javascript
setTextVerticalOverflow(value: TextOverflowType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOverflowType](../textoverflowtype/) | The value to set. |

### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}

<b>@deprecated.</b> Please use the 'textHorizontalOverflow' property instead. Gets and sets the text horizontal overflow type of the shape which contains text.

```javascript
getTextHorizontalOverflow() : TextOverflowType;
```


**Returns**

[TextOverflowType](../textoverflowtype/)

### setTextHorizontalOverflow(TextOverflowType) {#setTextHorizontalOverflow-textoverflowtype-}

<b>@deprecated.</b> Please use the 'textHorizontalOverflow' property instead. Gets and sets the text horizontal overflow type of the shape which contains text.

```javascript
setTextHorizontalOverflow(value: TextOverflowType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOverflowType](../textoverflowtype/) | The value to set. |

### isTextWrapped() {#isTextWrapped--}

<b>@deprecated.</b> Please use the 'isTextWrapped' property instead. Gets and sets the text wrapped type of the shape which contains text.

```javascript
isTextWrapped() : boolean;
```


### setIsTextWrapped(boolean) {#setIsTextWrapped-boolean-}

<b>@deprecated.</b> Please use the 'isTextWrapped' property instead. Gets and sets the text wrapped type of the shape which contains text.

```javascript
setIsTextWrapped(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextOrientationType() {#getTextOrientationType--}

<b>@deprecated.</b> Please use the 'textOrientationType' property instead. Gets and sets the text orientation type of the shape.

```javascript
getTextOrientationType() : TextOrientationType;
```


**Returns**

[TextOrientationType](../textorientationtype/)

### setTextOrientationType(TextOrientationType) {#setTextOrientationType-textorientationtype-}

<b>@deprecated.</b> Please use the 'textOrientationType' property instead. Gets and sets the text orientation type of the shape.

```javascript
setTextOrientationType(value: TextOrientationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOrientationType](../textorientationtype/) | The value to set. |

### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}

<b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment type of the shape.

```javascript
getTextHorizontalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextHorizontalAlignment(TextAlignmentType) {#setTextHorizontalAlignment-textalignmenttype-}

<b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment type of the shape.

```javascript
setTextHorizontalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getTextVerticalAlignment() {#getTextVerticalAlignment--}

<b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets and sets the text vertical alignment type of the shape.

```javascript
getTextVerticalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextVerticalAlignment(TextAlignmentType) {#setTextVerticalAlignment-textalignmenttype-}

<b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets and sets the text vertical alignment type of the shape.

```javascript
setTextVerticalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getTextDirection() {#getTextDirection--}

<b>@deprecated.</b> Please use the 'textDirection' property instead. Gets/Sets the direction of the text flow for this object.

```javascript
getTextDirection() : TextDirectionType;
```


**Returns**

[TextDirectionType](../textdirectiontype/)

### setTextDirection(TextDirectionType) {#setTextDirection-textdirectiontype-}

<b>@deprecated.</b> Please use the 'textDirection' property instead. Gets/Sets the direction of the text flow for this object.

```javascript
setTextDirection(value: TextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](../textdirectiontype/) | The value to set. |

### getTextBoxOptions() {#getTextBoxOptions--}

<b>@deprecated.</b> Please use the 'textBoxOptions' property instead. Gets the text information in the shape

```javascript
getTextBoxOptions() : TextBoxOptions;
```


**Returns**

[TextBoxOptions](../textboxoptions/)

### getControlData() {#getControlData--}

<b>@deprecated.</b> Please use the 'controlData' property instead. Gets the data of control.

```javascript
getControlData() : Uint8Array;
```


### getActiveXControl() {#getActiveXControl--}

<b>@deprecated.</b> Please use the 'activeXControl' property instead. Gets the ActiveX control.

```javascript
getActiveXControl() : ActiveXControl;
```


**Returns**

[ActiveXControl](../activexcontrol/)

### getPaths() {#getPaths--}

<b>@deprecated.</b> Please use the 'paths' property instead. Gets the paths of a custom geometric shape.

```javascript
getPaths() : ShapePathCollection;
```


**Returns**

[ShapePathCollection](../shapepathcollection/)

### getGeometry() {#getGeometry--}

<b>@deprecated.</b> Please use the 'geometry' property instead. Gets the geometry

```javascript
getGeometry() : Geometry;
```


**Returns**

[Geometry](../geometry/)

### isDecorative() {#isDecorative--}

<b>@deprecated.</b> Please use the 'isDecorative' property instead. Indicates whether the object is decorative.

```javascript
isDecorative() : boolean;
```


### setIsDecorative(boolean) {#setIsDecorative-boolean-}

<b>@deprecated.</b> Please use the 'isDecorative' property instead. Indicates whether the object is decorative.

```javascript
setIsDecorative(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### toFrontOrBack(number) {#toFrontOrBack-number-}

Brings the shape to the front or sends the shape to back.

```javascript
toFrontOrBack(orders: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| orders | number | If it's less than zero, sets the shape to back.         /// If it's greater than zero, brings the shape to front. |

### getLockedProperty(ShapeLockType) {#getLockedProperty-shapelocktype-}

Gets the value of locked property.

```javascript
getLockedProperty(type: ShapeLockType) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ShapeLockType](../shapelocktype/) | The type of the shape locked property. |

**Returns**

Returns  the value of locked property.

### setLockedProperty(ShapeLockType, boolean) {#setLockedProperty-shapelocktype-boolean-}

Set the locked property.

```javascript
setLockedProperty(type: ShapeLockType, value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ShapeLockType](../shapelocktype/) | The locked type. |
| value | boolean | The value of the property. |

### addHyperlink(string) {#addHyperlink-string-}

Adds a hyperlink to the shape.

```javascript
addHyperlink(address: string) : Hyperlink;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | string | Address of the hyperlink. |

**Returns**

Return the new hyperlink object.

### removeHyperlink() {#removeHyperlink--}

Removes the hyperlink of the shape.

```javascript
removeHyperlink() : void;
```


### moveToRange(number, number, number, number) {#moveToRange-number-number-number-number-}

Moves the shape to a specified range.

```javascript
moveToRange(topRow: number, leftColumn: number, bottomRow: number, rightColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| bottomRow | number | Lower right row index |
| rightColumn | number | Lower right column index |

### alignTopRightCorner(number, number) {#alignTopRightCorner-number-number-}

Moves the picture to the top-right corner.

```javascript
alignTopRightCorner(topRow: number, rightColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | the row index. |
| rightColumn | number | the column index. |

### getConnectionPoints() {#getConnectionPoints--}

Get the connection points

```javascript
getConnectionPoints() : number[][];
```


**Returns**

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### toImage(ImageType) {#toImage-imagetype-}

Creates the shape image and saves it to a stream in the specified format.

```javascript
toImage(imageType: ImageType) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageType | [ImageType](../imagetype/) | The type in which to save the image. |

**Returns**

The result stream

**Remarks**

The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### toImage(string, ImageOrPrintOptions) {#toImage-string-imageorprintoptions-}

Saves the shape to a file.

```javascript
toImage(imageFile: string, options: ImageOrPrintOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string |  |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

### toImage(ImageOrPrintOptions) {#toImage-imageorprintoptions-}

Saves the shape to a stream.

```javascript
toImage(options: ImageOrPrintOptions) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

**Returns**

The result stream

### toImageAsync(ImageType) {#toImageAsync-imagetype-}

Creates the shape image and saves it to a stream in the specified format.

```javascript
toImageAsync(imageType: ImageType) : Promise<Uint8Array>;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageType | [ImageType](../imagetype/) | The type in which to save the image. |

**Returns**

The result stream

**Remarks**

The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### toImageAsync(string, ImageOrPrintOptions) {#toImageAsync-string-imageorprintoptions-}

Saves the shape to a file.

```javascript
toImageAsync(imageFile: string, options: ImageOrPrintOptions) : Promise<void>;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string |  |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

**Returns**

[Promise<void>](../promise<void>/)

### toImageAsync(ImageOrPrintOptions) {#toImageAsync-imageorprintoptions-}

Saves the shape to a stream.

```javascript
toImageAsync(options: ImageOrPrintOptions) : Promise<Uint8Array>;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

**Returns**

The result stream

### getLinkedCell(boolean, boolean) {#getLinkedCell-boolean-boolean-}

Gets the range linked to the control's value.

```javascript
getLinkedCell(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The range linked to the control's value.

### setLinkedCell(string, boolean, boolean) {#setLinkedCell-string-boolean-boolean-}

Sets the range linked to the control's value.

```javascript
setLinkedCell(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The range linked to the control's value. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### getInputRange(boolean, boolean) {#getInputRange-boolean-boolean-}

Gets the range used to fill the control.

```javascript
getInputRange(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The range used to fill the control.

### setInputRange(string, boolean, boolean) {#setInputRange-string-boolean-boolean-}

Sets the range used to fill the control.

```javascript
setInputRange(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The range used to fill the control. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### updateSelectedValue() {#updateSelectedValue--}

Update the selected value by the value of the linked cell.

```javascript
updateSelectedValue() : void;
```


### calculateTextSize() {#calculateTextSize--}

Recalculate the text area

```javascript
calculateTextSize() : number[];
```


**Returns**

Text's Size in an array(width and height).

### formatCharacters(number, number, Font, StyleFlag) {#formatCharacters-number-number-font-styleflag-}

Formats some characters with the font setting.

```javascript
formatCharacters(startIndex: number, length: number, font: Font, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The start index. |
| length | number | The length. |
| font | [Font](../font/) | The font setting. |
| flag | [StyleFlag](../styleflag/) | The flag of the font setting. |

### characters(number, number) {#characters-number-number-}

Returns a Characters object that represents a range of characters within the text.

```javascript
characters(startIndex: number, length: number) : FontSetting;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the start of the character. |
| length | number | The number of characters. |

**Returns**

Characters object.

**Remarks**

This method only works on shape with title.

### getRichFormattings() {#getRichFormattings--}

Returns all Characters objects that represents a range of characters within the text .

```javascript
getRichFormattings() : FontSetting[];
```


**Returns**

All Characters objects

### removeActiveXControl() {#removeActiveXControl--}

Remove activeX control.

```javascript
removeActiveXControl() : void;
```


### getActualBox() {#getActualBox--}

Get the actual position and size of the shape (after applying rotation, flip, etc.)

```javascript
getActualBox() : number[];
```


**Returns**

Return the position and size in the order of x, y, w, h

**Remarks**

Note:The interface is not fully functional, especially the location information is not correct.It is recommended not to use this interface until the function is complete.

### fitToTextSize() {#fitToTextSize--}

Recalculate a text area suitable for displaying all text content.

```javascript
fitToTextSize() : void;
```


### getResultOfSmartArt() {#getResultOfSmartArt--}

Converting smart art to grouped shapes.

```javascript
getResultOfSmartArt() : GroupShape;
```


**Returns**

[GroupShape](../groupshape/)

### isSameSetting(Object) {#isSameSetting-object-}

Returns whether the shape is same.

```javascript
isSameSetting(obj: Object) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |


