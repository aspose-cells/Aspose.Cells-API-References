---
title: "Spinner Class"
linktitle: "Spinner"
articleTitle: "Spinner"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the Forms control: Spinner."
type: docs
weight: 6350
url: /python-java/asposecells.api/spinner/
---

## Spinner class

Represents the Forms control: Spinner.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CurrentValue](#currentvalue) | int | Gets or sets the current value. |
| [Min](#min) | int | Gets or sets the minimum value of a scroll bar or spinner range. |
| [Max](#max) | int | Gets or sets the maximum value of a scroll bar or spinner range. |
| [IncrementalChange](#incrementalchange) | int | Gets or sets the amount that the scroll bar or spinner is incremented a line scroll. |
| [Shadow](#shadow) | boolean | Indicates whether the shape has 3-D shading. |
| [IsHorizontal](#ishorizontal) | boolean | Indicates whether this is a horizontal scroll bar. |
| [MacroName](#macroname) | String | Gets and sets the name of macro. |
| [IsEquation](#isequation) | boolean | Indicates whether the shape only contains an equation. |
| [IsSmartArt](#issmartart) | boolean | Indicates whether the shape is a smart art. Only for ooxml file. |
| [ZOrderPosition](#zorderposition) | int | Returns the position of a shape in the z-order. |
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
| [SoftEdges](#softedges) | float | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [ThreeDFormat](#threedformat) | ThreeDFormat | Gets and sets 3d format of the shape. |
| [FormatPicture](#formatpicture) | MsoFormatPicture | Gets and sets the options of the picture format. |
| [IsHidden](#ishidden) | boolean | Indicates whether the object is visible. |
| [IsLockAspectRatio](#islockaspectratio) | boolean | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolet |
| [IsAspectRatioLocked](#isaspectratiolocked) | boolean | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. |
| [RotationAngle](#rotationangle) | float | Gets and sets the rotation of the shape. |
| [Hyperlink](#hyperlink) | Hyperlink | Gets the hyperlink of the shape. |
| [Id](#id) | int | Gets the identifier of this shape. |
| [Spid](#spid) | String | Specifies an optional string identifier that an application can use to identify the particular shape. |
| [Spt](#spt) | int | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [Worksheet](#worksheet) | Worksheet | Gets the Worksheet object which contains this shape. |
| [IsGroup](#isgroup) | boolean | Indicates whether this shape is a group shape. |
| [IsInGroup](#isingroup) | boolean | Indicates whether the shape is grouped. |
| [IsWordArt](#iswordart) | boolean | Indicates whether this shape is a word art. Only for the Legacy Shape of xls file. |
| [TextEffect](#texteffect) | TextEffectFormat | Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Sh |
| [IsLocked](#islocked) | boolean | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the wo |
| [IsPrintable](#isprintable) | boolean | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [MsoDrawingType](#msodrawingtype) | int | Gets drawing type. The value of the property is MsoDrawingType integer constant. |
| [AutoShapeType](#autoshapetype) | int | Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant. |
| [AnchorType](#anchortype) | int | Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant. |
| [Placement](#placement) | int | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an objec |
| [UpperLeftRow](#upperleftrow) | int | Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored. |
| [UpperDeltaY](#upperdeltay) | int | Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256. |
| [UpperLeftColumn](#upperleftcolumn) | int | Represents upper left corner column index. |
| [UpperDeltaX](#upperdeltax) | int | Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024. |
| [LowerRightRow](#lowerrightrow) | int | Represents lower right corner row index. |
| [LowerDeltaY](#lowerdeltay) | int | Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256. |
| [LowerRightColumn](#lowerrightcolumn) | int | Represents lower right corner column index. |
| [LowerDeltaX](#lowerdeltax) | int | Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024. |
| [Right](#right) | int | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [Bottom](#bottom) | int | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [Width](#width) | int | Represents the width of shape, in unit of pixels. |
| [WidthInch](#widthinch) | float | Represents the width of the shape, in unit of inch. |
| [WidthPt](#widthpt) | float | Represents the width of the shape, in unit of point. |
| [WidthCM](#widthcm) | float | Represents the width of the shape, in unit of centimeters. |
| [Height](#height) | int | Represents the height of shape, in unit of pixel. |
| [HeightInch](#heightinch) | float | Represents the height of the shape, in unit of inches. |
| [HeightPt](#heightpt) | float | Represents the height of the shape, in unit of points. |
| [HeightCM](#heightcm) | float | Represents the height of the shape, in unit of centimeters. |
| [Left](#left) | int | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [LeftInch](#leftinch) | float | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [LeftCM](#leftcm) | float | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [Top](#top) | int | Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents th |
| [TopInch](#topinch) | float | Represents the vertical offset of shape from its top row, in unit of inches. |
| [TopCM](#topcm) | float | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [TopToCorner](#toptocorner) | int | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [LeftToCorner](#lefttocorner) | int | Gets and sets the horizonal offset of shape from worksheet left border. |
| [X](#x) | int | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [Y](#y) | int | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [WidthScale](#widthscale) | int | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthS |
| [HeightScale](#heightscale) | int | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the Heigh |
| [TopInShape](#topinshape) | int | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [LeftInShape](#leftinshape) | int | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the pa |
| [WidthInShape](#widthinshape) | int | Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or c |
| [HeightInShape](#heightinshape) | int | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [Group](#group) | GroupShape | Gets the group shape which contains this shape. |
| [Type](#type) | int | Gets the auto shape type. The value of the property is AutoShapeType integer constant. |
| [HasLine](#hasline) | boolean | Gets and sets the line border of the shape is visible. |
| [IsFilled](#isfilled) | boolean | Indicates whether the fill format is visible. |
| [IsFlippedHorizontally](#isflippedhorizontally) | boolean | Gets and sets whether shape is horizontally flipped . |
| [IsFlippedVertically](#isflippedvertically) | boolean | Gets and sets whether shape is vertically flipped . |
| [ActualLowerRightRow](#actuallowerrightrow) | int | Get the actual bottom row. |
| [RelativeToOriginalPictureSize](#relativetooriginalpicturesize) | boolean | Indicates whether shape is relative to original picture size. |
| [LinkedCell](#linkedcell) | String | Gets or sets the worksheet range linked to the control's value. |
| [InputRange](#inputrange) | String | Gets or sets the worksheet range used to fill the specified combo box. |
| [TextShapeType](#textshapetype) | int | Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant. |
| [TextBody](#textbody) | FontSettingCollection | Gets and sets the setting of the shape's text. |
| [Font](#font) | Font | Represents the font of shape. |
| [TextOptions](#textoptions) | TextOptions | Represents the text options of the shape. |
| [Text](#text) | String | Gets and sets the text of this shape. |
| [IsRichText](#isrichtext) | boolean | Whether or not the text is rich text. |
| [HtmlText](#htmltext) | String | Gets and sets the html string which contains data and some formats in this textbox. |
| [TextVerticalOverflow](#textverticaloverflow) | int | Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflo |
| [TextHorizontalOverflow](#texthorizontaloverflow) | int | Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverf |
| [IsTextWrapped](#istextwrapped) | boolean | Gets and sets the text wrapped type of the shape which contains text. |
| [TextOrientationType](#textorientationtype) | int | Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant. |
| [TextHorizontalAlignment](#texthorizontalalignment) | int | Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer co |
| [TextVerticalAlignment](#textverticalalignment) | int | Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer cons |
| [TextDirection](#textdirection) | int | Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constan |
| [TextBoxOptions](#textboxoptions) | TextBoxOptions |  |
| [ControlData](#controldata) | byte[] | Gets the data of control. |
| [Paths](#paths) | ShapePathCollection | Gets the paths of a custom geometric shape. |
| [Geometry](#geometry) | Geometry | Gets the geometry |
| [CreateId](#createid) | UUID | Gets and sets create id for this shape. |
| [IsDecorative](#isdecorative) | boolean | Indicates whether the object is decorative. |

## Methods

| Name | Description |
| --- | --- |
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

### Spinner.CurrentValue property {#currentvalue}

Gets or sets the current value.

**Type:** int

### Spinner.Min property {#min}

Gets or sets the minimum value of a scroll bar or spinner range.

**Type:** int

### Spinner.Max property {#max}

Gets or sets the maximum value of a scroll bar or spinner range.

**Type:** int

### Spinner.IncrementalChange property {#incrementalchange}

Gets or sets the amount that the scroll bar or spinner is incremented a line scroll.

**Type:** int

### Spinner.Shadow property {#shadow}

Indicates whether the shape has 3-D shading.

**Type:** boolean

### Spinner.IsHorizontal property {#ishorizontal}

Indicates whether this is a horizontal scroll bar.

**Type:** boolean

### Spinner.MacroName property {#macroname}

Gets and sets the name of macro.

**Type:** String

### Spinner.IsEquation property {#isequation}

Indicates whether the shape only contains an equation.

**Type:** boolean

### Spinner.IsSmartArt property {#issmartart}

Indicates whether the shape is a smart art. Only for ooxml file.

**Type:** boolean

### Spinner.ZOrderPosition property {#zorderposition}

Returns the position of a shape in the z-order.

**Type:** int

### Spinner.Name property {#name}

Gets and sets the name of the shape.

**Type:** String

### Spinner.AlternativeText property {#alternativetext}

Returns or sets the descriptive (alternative) text string of the Shape object.

**Type:** String

### Spinner.Title property {#title}

Specifies the title (caption) of the current shape object.

**Type:** String

### Spinner.LineFormat property {#lineformat}

Returns a MsoLineFormat object that contains line formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** MsoLineFormat

### Spinner.FillFormat property {#fillformat}

Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** MsoFillFormat

### Spinner.Line property {#line}

Gets line style

**Type:** LineFormat

### Spinner.Fill property {#fill}

Returns a FillFormat object that contains fill formatting properties for the specified shape.

**Type:** FillFormat

### Spinner.ShadowEffect property {#shadoweffect}

Represents a ShadowEffect object that specifies shadow effect for the chart element or shape.

**Type:** ShadowEffect

### Spinner.Reflection property {#reflection}

Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape.

**Type:** ReflectionEffect

### Spinner.Glow property {#glow}

Represents a GlowEffect object that specifies glow effect for the chart element or shape.

**Type:** GlowEffect

### Spinner.SoftEdges property {#softedges}

Gets and sets the radius of blur to apply to the edges, in unit of points.

**Type:** float

### Spinner.ThreeDFormat property {#threedformat}

Gets and sets 3d format of the shape.

**Type:** ThreeDFormat

### Spinner.FormatPicture property {#formatpicture}

Gets and sets the options of the picture format.

**Type:** MsoFormatPicture

### Spinner.IsHidden property {#ishidden}

Indicates whether the object is visible.

**Type:** boolean

### Spinner.IsLockAspectRatio property {#islockaspectratio}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### Spinner.IsAspectRatioLocked property {#isaspectratiolocked}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects.

**Type:** boolean

### Spinner.RotationAngle property {#rotationangle}

Gets and sets the rotation of the shape.

**Type:** float

### Spinner.Hyperlink property {#hyperlink}

Gets the hyperlink of the shape.

**Type:** Hyperlink

### Spinner.Id property {#id}

Gets the identifier of this shape.

**Type:** int

### Spinner.Spid property {#spid}

Specifies an optional string identifier that an application can use to identify the particular shape.

**Type:** String

### Spinner.Spt property {#spt}

Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

**Type:** int

### Spinner.Worksheet property {#worksheet}

Gets the Worksheet object which contains this shape.

**Type:** Worksheet

### Spinner.IsGroup property {#isgroup}

Indicates whether this shape is a group shape.

**Type:** boolean

### Spinner.IsInGroup property {#isingroup}

Indicates whether the shape is grouped.

**Type:** boolean

### Spinner.IsWordArt property {#iswordart}

Indicates whether this shape is a word art. Only for the Legacy Shape of xls file.

**Type:** boolean

### Spinner.TextEffect property {#texteffect}

Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

**Type:** TextEffectFormat

### Spinner.IsLocked property {#islocked}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

**Type:** boolean

### Spinner.IsPrintable property {#isprintable}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

**Type:** boolean

### Spinner.MsoDrawingType property {#msodrawingtype}

Gets drawing type. The value of the property is MsoDrawingType integer constant.

**Type:** int

### Spinner.AutoShapeType property {#autoshapetype}

Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant.

**Type:** int

### Spinner.AnchorType property {#anchortype}

Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant.

**Type:** int

### Spinner.Placement property {#placement}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. The value of the property is PlacementType integer constant.

**Type:** int

### Spinner.UpperLeftRow property {#upperleftrow}

Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

**Type:** int

### Spinner.UpperDeltaY property {#upperdeltay}

Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

**Type:** int

### Spinner.UpperLeftColumn property {#upperleftcolumn}

Represents upper left corner column index.

**Type:** int

### Spinner.UpperDeltaX property {#upperdeltax}

Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

**Type:** int

### Spinner.LowerRightRow property {#lowerrightrow}

Represents lower right corner row index.

**Type:** int

### Spinner.LowerDeltaY property {#lowerdeltay}

Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

**Type:** int

### Spinner.LowerRightColumn property {#lowerrightcolumn}

Represents lower right corner column index.

**Type:** int

### Spinner.LowerDeltaX property {#lowerdeltax}

Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

**Type:** int

### Spinner.Right property {#right}

Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

**Type:** int

### Spinner.Bottom property {#bottom}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

**Type:** int

### Spinner.Width property {#width}

Represents the width of shape, in unit of pixels.

**Type:** int

### Spinner.WidthInch property {#widthinch}

Represents the width of the shape, in unit of inch.

**Type:** float

### Spinner.WidthPt property {#widthpt}

Represents the width of the shape, in unit of point.

**Type:** float

### Spinner.WidthCM property {#widthcm}

Represents the width of the shape, in unit of centimeters.

**Type:** float

### Spinner.Height property {#height}

Represents the height of shape, in unit of pixel.

**Type:** int

### Spinner.HeightInch property {#heightinch}

Represents the height of the shape, in unit of inches.

**Type:** float

### Spinner.HeightPt property {#heightpt}

Represents the height of the shape, in unit of points.

**Type:** float

### Spinner.HeightCM property {#heightcm}

Represents the height of the shape, in unit of centimeters.

**Type:** float

### Spinner.Left property {#left}

Represents the horizontal offset of shape from its left column, in unit of pixels.

**Type:** int

### Spinner.LeftInch property {#leftinch}

Represents the horizontal offset of shape from its left column, in unit of inches.

**Type:** float

### Spinner.LeftCM property {#leftcm}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

**Type:** float

### Spinner.Top property {#top}

Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

**Type:** int

### Spinner.TopInch property {#topinch}

Represents the vertical offset of shape from its top row, in unit of inches.

**Type:** float

### Spinner.TopCM property {#topcm}

Represents the vertical offset of shape from its top row, in unit of centimeters.

**Type:** float

### Spinner.TopToCorner property {#toptocorner}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

**Type:** int

### Spinner.LeftToCorner property {#lefttocorner}

Gets and sets the horizonal offset of shape from worksheet left border.

**Type:** int

### Spinner.X property {#x}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

**Type:** int

### Spinner.Y property {#y}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

**Type:** int

### Spinner.WidthScale property {#widthscale}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

**Type:** int

### Spinner.HeightScale property {#heightscale}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

**Type:** int

### Spinner.TopInShape property {#topinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. Only Applies when this shape in the group or chart.

**Type:** int

### Spinner.LeftInShape property {#leftinshape}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. Only Applies when this shape in the group or chart.

**Type:** int

### Spinner.WidthInShape property {#widthinshape}

Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or chart.

**Type:** int

### Spinner.HeightInShape property {#heightinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. Only Applies when this shape in the group or chart.

**Type:** int

### Spinner.Group property {#group}

Gets the group shape which contains this shape.

**Type:** GroupShape

### Spinner.Type property {#type}

Gets the auto shape type. The value of the property is AutoShapeType integer constant.

**Type:** int

### Spinner.HasLine property {#hasline}

Gets and sets the line border of the shape is visible.

**Type:** boolean

### Spinner.IsFilled property {#isfilled}

Indicates whether the fill format is visible.

**Type:** boolean

### Spinner.IsFlippedHorizontally property {#isflippedhorizontally}

Gets and sets whether shape is horizontally flipped .

**Type:** boolean

### Spinner.IsFlippedVertically property {#isflippedvertically}

Gets and sets whether shape is vertically flipped .

**Type:** boolean

### Spinner.ActualLowerRightRow property {#actuallowerrightrow}

Get the actual bottom row.

**Type:** int

### Spinner.RelativeToOriginalPictureSize property {#relativetooriginalpicturesize}

Indicates whether shape is relative to original picture size.

**Type:** boolean

### Spinner.LinkedCell property {#linkedcell}

Gets or sets the worksheet range linked to the control's value.

**Type:** String

### Spinner.InputRange property {#inputrange}

Gets or sets the worksheet range used to fill the specified combo box.

**Type:** String

### Spinner.TextShapeType property {#textshapetype}

Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant.

**Type:** int

### Spinner.TextBody property {#textbody}

Gets and sets the setting of the shape's text.

**Type:** FontSettingCollection

### Spinner.Font property {#font}

Represents the font of shape.

**Type:** Font

### Spinner.TextOptions property {#textoptions}

Represents the text options of the shape.

**Type:** TextOptions

### Spinner.Text property {#text}

Gets and sets the text of this shape.

**Type:** String

### Spinner.IsRichText property {#isrichtext}

Whether or not the text is rich text.

**Type:** boolean

### Spinner.HtmlText property {#htmltext}

Gets and sets the html string which contains data and some formats in this textbox.

**Type:** String

### Spinner.TextVerticalOverflow property {#textverticaloverflow}

Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

**Type:** int

### Spinner.TextHorizontalOverflow property {#texthorizontaloverflow}

Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

**Type:** int

### Spinner.IsTextWrapped property {#istextwrapped}

Gets and sets the text wrapped type of the shape which contains text.

**Type:** boolean

### Spinner.TextOrientationType property {#textorientationtype}

Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant.

**Type:** int

### Spinner.TextHorizontalAlignment property {#texthorizontalalignment}

Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer constant.

**Type:** int

### Spinner.TextVerticalAlignment property {#textverticalalignment}

Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer constant.

**Type:** int

### Spinner.TextDirection property {#textdirection}

Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constant.

**Type:** int

### Spinner.TextBoxOptions property {#textboxoptions}

**Type:** TextBoxOptions

### Spinner.ControlData property {#controldata}

Gets the data of control.

**Type:** byte[]

### Spinner.Paths property {#paths}

Gets the paths of a custom geometric shape.

**Type:** ShapePathCollection

### Spinner.Geometry property {#geometry}

Gets the geometry

**Type:** Geometry

### Spinner.CreateId property {#createid}

Gets and sets create id for this shape.

**Type:** UUID

### Spinner.IsDecorative property {#isdecorative}

Indicates whether the object is decorative.

**Type:** boolean

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
| startIndex | int | The start index. |
| length | int | The length. |
| font | Font | The font setting. |
| flag | StyleFlag | The flag of the font setting. |

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the text.

This method only works on shape with title.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |

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
| orders | int | If it's less than zero, sets the shape to back. If it's greater than zero, brings the shape to front. |

### getLockedProperty(type) {#getlockedproperty}

Gets the value of locked property.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ShapeLockType value. The type of the shape locked property. |

**Returns:** Returns the value of locked property.

### setLockedProperty(type, value) {#setlockedproperty}

Set the locked property.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ShapeLockType value. The locked type. |
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
| topRow | int | the row index. |
| rightColumn | int | the column index. |
