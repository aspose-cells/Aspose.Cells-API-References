##CustomXmlShape Class
'CustomXmlShape class. Encapsulates the object that represents customxmlshape in Go.'
## CustomXmlShape class
Represents Custom xml shape ,such as Ink.
```go
type CustomXmlShape struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCustomXmlShape](./newcustomxmlshape/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetMacroName](./getmacroname/) | Gets and sets the name of macro. |
|[SetMacroName](./setmacroname/) | Gets and sets the name of macro. |
|[IsEquation](./isequation/) | Indicates whether the shape only contains an equation. |
|[IsSmartArt](./issmartart/) | Indicates whether the shape is a smart art. |
|[ToFrontOrBack](./tofrontorback/) | Brings the shape to the front or sends the shape to back. |
|[GetZOrderPosition](./getzorderposition/) | Returns the position of a shape in the z-order. |
|[SetZOrderPosition](./setzorderposition/) | Returns the position of a shape in the z-order. |
|[GetName](./getname/) | Gets and sets the name of the shape. |
|[SetName](./setname/) | Gets and sets the name of the shape. |
|[GetAlternativeText](./getalternativetext/) | Returns or sets the descriptive (alternative) text string of the Shape object. |
|[SetAlternativeText](./setalternativetext/) | Returns or sets the descriptive (alternative) text string of the Shape object. |
|[GetTitle](./gettitle/) | Specifies the title (caption) of the current shape object. |
|[SetTitle](./settitle/) | Specifies the title (caption) of the current shape object. |
|[GetLine](./getline/) | Gets line style |
|[GetFill](./getfill/) | Returns a FillFormat object that contains fill formatting properties for the specified shape. |
|[GetShadowEffect](./getshadoweffect/) | Represents a Drawing.ShadowEffect object that specifies shadow effect for the chart element or shape. |
|[GetReflection](./getreflection/) | Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape. |
|[GetGlow](./getglow/) | Represents a GlowEffect object that specifies glow effect for the chart element or shape. |
|[GetSoftEdges](./getsoftedges/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
|[SetSoftEdges](./setsoftedges/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
|[GetThreeDFormat](./getthreedformat/) | Gets and sets 3d format of the shape. |
|[GetFormatPicture](./getformatpicture/) | Gets and sets the options of the picture format. |
|[IsHidden](./ishidden/) | Indicates whether the object is visible. |
|[SetIsHidden](./setishidden/) | Indicates whether the object is visible. |
|[IsAspectRatioLocked](./isaspectratiolocked/) | True means that aspect ratio of the shape is locked. |
|[SetIsAspectRatioLocked](./setisaspectratiolocked/) | True means that aspect ratio of the shape is locked. |
|[GetLockedProperty](./getlockedproperty/) | Gets the value of locked property. |
|[SetLockedProperty](./setlockedproperty/) | Set the locked property. |
|[GetRotationAngle](./getrotationangle/) | Gets and sets the rotation of the shape. |
|[SetRotationAngle](./setrotationangle/) | Gets and sets the rotation of the shape. |
|[AddHyperlink](./addhyperlink/) | Adds a hyperlink to the shape. |
|[RemoveHyperlink](./removehyperlink/) | Removes the hyperlink of the shape. |
|[GetHyperlink](./gethyperlink/) | Gets the hyperlink of the shape. |
|[MoveToRange](./movetorange/) | Moves the shape to a specified range. |
|[AlignTopRightCorner](./aligntoprightcorner/) | Moves the picture to the top-right corner. |
|[GetId](./getid/) | Gets the identifier of this shape. |
|[GetSpid](./getspid/) | Specifies an optional string identifier that an application can use to identify the particular shape. |
|[GetSpt](./getspt/) | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
|[GetWorksheet](./getworksheet/) | Gets the Worksheet object which contains this shape. |
|[IsGroup](./isgroup/) | Indicates whether this shape is a group shape. |
|[IsInGroup](./isingroup/) | Indicates whether the shape is grouped. |
|[IsWordArt](./iswordart/) | Indicates whether this shape is a word art. |
|[GetTextEffect](./gettexteffect/) | Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape.Applies to Shape objects that represent WordArt. |
|[IsLocked](./islocked/) | True means the object can not be modified when the sheet is protected.Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
|[SetIsLocked](./setislocked/) | True means the object can not be modified when the sheet is protected.Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
|[IsPrintable](./isprintable/) | Indicates whether the object is printable.If False, this shape will not be printed when printing. |
|[SetIsPrintable](./setisprintable/) | Indicates whether the object is printable.If False, this shape will not be printed when printing. |
|[GetMsoDrawingType](./getmsodrawingtype/) | Gets drawing type. |
|[GetAutoShapeType](./getautoshapetype/) | Gets and sets the auto shape type. |
|[SetAutoShapeType](./setautoshapetype/) | Gets and sets the auto shape type. |
|[GetAnchorType](./getanchortype/) | Gets and set the type of the shape anchor placeholder. |
|[SetAnchorType](./setanchortype/) | Gets and set the type of the shape anchor placeholder. |
|[GetPlacement](./getplacement/) | Represents the way the drawing object is attached to the cells below it.The property controls the placement of an object on a worksheet. |
|[SetPlacement](./setplacement/) | Represents the way the drawing object is attached to the cells below it.The property controls the placement of an object on a worksheet. |
|[GetUpperLeftRow](./getupperleftrow/) | Represents the top row index. |
|[SetUpperLeftRow](./setupperleftrow/) | Represents the top row index. |
|[GetUpperDeltaY](./getupperdeltay/) | Gets or sets the shape's vertical offset from its upper left corner row. |
|[SetUpperDeltaY](./setupperdeltay/) | Gets or sets the shape's vertical offset from its upper left corner row. |
|[GetUpperLeftColumn](./getupperleftcolumn/) | Represents upper left corner column index. |
|[SetUpperLeftColumn](./setupperleftcolumn/) | Represents upper left corner column index. |
|[GetUpperDeltaX](./getupperdeltax/) | Gets or sets the shape's horizontal offset from its upper left corner column. |
|[SetUpperDeltaX](./setupperdeltax/) | Gets or sets the shape's horizontal offset from its upper left corner column. |
|[GetLowerRightRow](./getlowerrightrow/) | Represents lower right corner row index. |
|[SetLowerRightRow](./setlowerrightrow/) | Represents lower right corner row index. |
|[GetLowerDeltaY](./getlowerdeltay/) | Gets or sets the shape's vertical offset from its lower right corner row. |
|[SetLowerDeltaY](./setlowerdeltay/) | Gets or sets the shape's vertical offset from its lower right corner row. |
|[GetLowerRightColumn](./getlowerrightcolumn/) | Represents lower right corner column index. |
|[SetLowerRightColumn](./setlowerrightcolumn/) | Represents lower right corner column index. |
|[GetLowerDeltaX](./getlowerdeltax/) | Gets or sets the shape's horizontal  offset from its lower right corner column. |
|[SetLowerDeltaX](./setlowerdeltax/) | Gets or sets the shape's horizontal  offset from its lower right corner column. |
|[GetRight](./getright/) | Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
|[SetRight](./setright/) | Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
|[GetBottom](./getbottom/) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
|[SetBottom](./setbottom/) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
|[GetWidth](./getwidth/) | Represents the width of shape, in unit of pixels. |
|[SetWidth](./setwidth/) | Represents the width of shape, in unit of pixels. |
|[GetWidthInch](./getwidthinch/) | Represents the width of the shape, in unit of inch. |
|[SetWidthInch](./setwidthinch/) | Represents the width of the shape, in unit of inch. |
|[GetWidthPt](./getwidthpt/) | Represents the width of the shape, in unit of point. |
|[SetWidthPt](./setwidthpt/) | Represents the width of the shape, in unit of point. |
|[GetWidthCM](./getwidthcm/) | Represents the width of the shape, in unit of centimeters. |
|[SetWidthCM](./setwidthcm/) | Represents the width of the shape, in unit of centimeters. |
|[GetHeight](./getheight/) | Represents the height of shape, in unit of pixel. |
|[SetHeight](./setheight/) | Represents the height of shape, in unit of pixel. |
|[GetHeightInch](./getheightinch/) | Represents the height of the shape, in unit of inches. |
|[SetHeightInch](./setheightinch/) | Represents the height of the shape, in unit of inches. |
|[GetHeightPt](./getheightpt/) | Represents the height of the shape, in unit of points. |
|[SetHeightPt](./setheightpt/) | Represents the height of the shape, in unit of points. |
|[GetHeightCM](./getheightcm/) | Represents the height of the shape, in unit of centimeters. |
|[SetHeightCM](./setheightcm/) | Represents the height of the shape, in unit of centimeters. |
|[GetLeft](./getleft/) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
|[SetLeft](./setleft/) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
|[GetLeftInch](./getleftinch/) | Represents the horizontal offset of shape from its left column, in unit of inches. |
|[SetLeftInch](./setleftinch/) | Represents the horizontal offset of shape from its left column, in unit of inches. |
|[GetLeftCM](./getleftcm/) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
|[SetLeftCM](./setleftcm/) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
|[GetTop](./gettop/) | Represents the vertical offset of shape from its top row, in unit of pixels. |
|[SetTop](./settop/) | Represents the vertical offset of shape from its top row, in unit of pixels. |
|[GetTopInch](./gettopinch/) | Represents the vertical offset of shape from its top row, in unit of inches. |
|[SetTopInch](./settopinch/) | Represents the vertical offset of shape from its top row, in unit of inches. |
|[GetTopCM](./gettopcm/) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
|[SetTopCM](./settopcm/) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
|[GetTopToCorner](./gettoptocorner/) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
|[SetTopToCorner](./settoptocorner/) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
|[GetLeftToCorner](./getlefttocorner/) | Gets and sets the horizonal offset of shape from worksheet left border. |
|[SetLeftToCorner](./setlefttocorner/) | Gets and sets the horizonal offset of shape from worksheet left border. |
|[GetX](./getx/) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
|[SetX](./setx/) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
|[GetY](./gety/) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
|[SetY](./sety/) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
|[GetWidthScale](./getwidthscale/) | Gets and sets the width scale, in unit of percent of the original picture width.If the shape is not picture ,the WidthScale property only returns 100; |
|[SetWidthScale](./setwidthscale/) | Gets and sets the width scale, in unit of percent of the original picture width.If the shape is not picture ,the WidthScale property only returns 100; |
|[GetHeightScale](./getheightscale/) | Gets and sets the height scale,in unit of percent of the original picture height.If the shape is not picture ,the HeightScale property only returns 100; |
|[SetHeightScale](./setheightscale/) | Gets and sets the height scale,in unit of percent of the original picture height.If the shape is not picture ,the HeightScale property only returns 100; |
|[GetTopInShape](./gettopinshape/) | Represents the vertical offset of shape from the top border of the parent shape,in unit of 1/4000 of height of the parent shape. |
|[SetTopInShape](./settopinshape/) | Represents the vertical offset of shape from the top border of the parent shape,in unit of 1/4000 of height of the parent shape. |
|[GetLeftInShape](./getleftinshape/) | Represents the horizontal offset of shape from the left border of the parent shape,in unit of 1/4000 of width of the parent shape. |
|[SetLeftInShape](./setleftinshape/) | Represents the horizontal offset of shape from the left border of the parent shape,in unit of 1/4000 of width of the parent shape. |
|[GetWidthInShape](./getwidthinshape/) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
|[SetWidthInShape](./setwidthinshape/) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
|[GetHeightInShape](./getheightinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
|[SetHeightInShape](./setheightinshape/) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
|[GetGroup](./getgroup/) | Gets the group shape which contains this shape. |
|[GetType](./gettype/) | Gets the auto shape type. |
|[GetHasLine](./gethasline/) | Gets and sets the line border of the shape is visible. |
|[SetHasLine](./sethasline/) | Gets and sets the line border of the shape is visible. |
|[IsFilled](./isfilled/) | Indicates whether the fill format is visible. |
|[SetIsFilled](./setisfilled/) | Indicates whether the fill format is visible. |
|[IsFlippedHorizontally](./isflippedhorizontally/) | Gets and sets whether shape is horizontally flipped . |
|[SetIsFlippedHorizontally](./setisflippedhorizontally/) | Gets and sets whether shape is horizontally flipped . |
|[IsFlippedVertically](./isflippedvertically/) | Gets and sets whether shape is vertically flipped . |
|[SetIsFlippedVertically](./setisflippedvertically/) | Gets and sets whether shape is vertically flipped . |
|[GetActualLowerRightRow](./getactuallowerrightrow/) | Get the actual bottom row. |
|[GetConnectionPoints](./getconnectionpoints/) | Get the connection points |
|[ToImage_ImageType](./toimage_imagetype/) | Creates the shape image and saves it to a stream in the specified format. |
|[ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Saves the shape to a file. |
|[ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Saves the shape to a stream. |
|[GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | Indicates whether shape is relative to original picture size. |
|[SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | Indicates whether shape is relative to original picture size. |
|[GetLinkedCell](./getlinkedcell/) | Gets or sets the worksheet range linked to the control's value. |
|[SetLinkedCell_String](./setlinkedcell_string/) | Gets or sets the worksheet range linked to the control's value. |
|[GetInputRange](./getinputrange/) | Gets or sets the worksheet range used to fill the specified combo box. |
|[SetInputRange_String](./setinputrange_string/) | Gets or sets the worksheet range used to fill the specified combo box. |
|[GetLinkedCell_Bool_Bool](./getlinkedcell_bool_bool/) | Gets the range linked to the control's value. |
|[SetLinkedCell_String_Bool_Bool](./setlinkedcell_string_bool_bool/) | Sets the range linked to the control's value. |
|[GetInputRange_Bool_Bool](./getinputrange_bool_bool/) | Gets the range used to fill the control. |
|[SetInputRange_String_Bool_Bool](./setinputrange_string_bool_bool/) | Sets the range used to fill the control. |
|[UpdateSelectedValue](./updateselectedvalue/) | Update the selected value by the value of the linked cell. |
|[GetTextShapeType](./gettextshapetype/) | Gets and sets the preset text shape type. |
|[SetTextShapeType](./settextshapetype/) | Gets and sets the preset text shape type. |
|[GetTextBody](./gettextbody/) | Gets and sets the setting of the shape's text. |
|[GetFont](./getfont/) | Represents the font of shape. |
|[SetFont](./setfont/) | Represents the font of shape. |
|[GetTextOptions](./gettextoptions/) | Represents the text options of the shape. |
|[SetTextOptions](./settextoptions/) | Represents the text options of the shape. |
|[CalculateTextSize](./calculatetextsize/) | Recalculate the text area |
|[GetText](./gettext/) | Gets and sets the text of this shape. |
|[SetText](./settext/) | Gets and sets the text of this shape. |
|[IsRichText](./isrichtext/) | Whether or not the text is rich text. |
|[GetHtmlText](./gethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
|[SetHtmlText](./sethtmltext/) | Gets and sets the html string which contains data and some formats in this textbox. |
|[FormatCharacters](./formatcharacters/) | Formats some characters with the font setting. |
|[Characters](./characters/) | Returns a Characters object that represents a range of characters within the text. |
|[GetRichFormattings](./getrichformattings/) | Returns all Characters objectsthat represents a range of characters within the text . |
|[GetTextVerticalOverflow](./gettextverticaloverflow/) | Gets and sets the text vertical overflow type of the shape which contains text. |
|[SetTextVerticalOverflow](./settextverticaloverflow/) | Gets and sets the text vertical overflow type of the shape which contains text. |
|[GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the shape which contains text. |
|[SetTextHorizontalOverflow](./settexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the shape which contains text. |
|[IsTextWrapped](./istextwrapped/) | Gets and sets the text wrapped type of the shape which contains text. |
|[SetIsTextWrapped](./setistextwrapped/) | Gets and sets the text wrapped type of the shape which contains text. |
|[GetTextOrientationType](./gettextorientationtype/) | Gets and sets the text orientation type of the shape. |
|[SetTextOrientationType](./settextorientationtype/) | Gets and sets the text orientation type of the shape. |
|[GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the shape. |
|[SetTextHorizontalAlignment](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the shape. |
|[GetTextVerticalAlignment](./gettextverticalalignment/) | Gets and sets the text vertical alignment type of the shape. |
|[SetTextVerticalAlignment](./settextverticalalignment/) | Gets and sets the text vertical alignment type of the shape. |
|[GetTextDirection](./gettextdirection/) | Gets/Sets the direction of the text flow for this object. |
|[SetTextDirection](./settextdirection/) | Gets/Sets the direction of the text flow for this object. |
|[GetTextBoxOptions](./gettextboxoptions/) | Gets the text information in the shape |
|[GetControlData](./getcontroldata/) | Gets the data of control. |
|[GetActiveXControl](./getactivexcontrol/) | Gets the ActiveX control. |
|[RemoveActiveXControl](./removeactivexcontrol/) | Remove activeX control. |
|[GetPaths](./getpaths/) | Gets the paths of a custom geometric shape. |
|[GetGeometry](./getgeometry/) | Gets the geometry |
|[GetCreateId](./getcreateid/) | Gets and sets create id for this shape. |
|[SetCreateId](./setcreateid/) | Gets and sets create id for this shape. |
|[IsDecorative](./isdecorative/) | Indicates whether the object is decorative. |
|[SetIsDecorative](./setisdecorative/) | Indicates whether the object is decorative. |
|[GetActualBox](./getactualbox/) | Get the actual position and size of the shape (after applying rotation, flip, etc.) |
|[FitToTextSize](./fittotextsize/) | Recalculate a text area suitable for displaying all text content. |
|[GetResultOfSmartArt](./getresultofsmartart/) | Converting smart art to grouped shapes. |
|[IsSameSetting](./issamesetting/) | Returns whether the shape is same. |
