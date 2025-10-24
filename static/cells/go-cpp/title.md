##Title Class
'Title class. Encapsulates the object that represents title in Go.'
## Title class
Encapsulates the object that represents the title of chart or axis.
```go
type Title struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTitle](./newtitle/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetText](./gettext/) | Gets or sets the text of display unit label. |
|[SetText](./settext/) | Gets or sets the text of display unit label. |
|[IsVisible](./isvisible/) | Represents whether the title is visible. |
|[SetIsVisible](./setisvisible/) | Represents whether the title is visible. |
|[GetXRatioToChart](./getxratiotochart/) | Gets or sets the x coordinate of the upper left corner in units of Fraction of the chart area.X In Pixels = XRatioToChart * Chart.ChartObject.Width; |
|[SetXRatioToChart](./setxratiotochart/) | Gets or sets the x coordinate of the upper left corner in units of Fraction of the chart area.X In Pixels = XRatioToChart * Chart.ChartObject.Width; |
|[GetYRatioToChart](./getyratiotochart/) | Gets or sets the y coordinate of the upper left corner in units of Fraction of the chart area.Y In Pixels = YRatioToChart * Chart.ChartObject.Width; |
|[SetYRatioToChart](./setyratiotochart/) | Gets or sets the y coordinate of the upper left corner in units of Fraction of the chart area.Y In Pixels = YRatioToChart * Chart.ChartObject.Width; |
|[GetOverLay](./getoverlay/) | Represents overlay centered title on chart without resizing chart. |
|[SetOverLay](./setoverlay/) | Represents overlay centered title on chart without resizing chart. |
|[Characters](./characters/) | Gets rich text formatting of this Title. |
|[Characters_Int_Int](./characters_int_int/) | Returns a Characters object that represents a range of characters within the text. |
|[IsInnerMode](./isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
|[SetIsInnerMode](./setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
|[GetBackgroundMode](./getbackgroundmode/) | Gets and sets the display mode of the background |
|[SetBackgroundMode](./setbackgroundmode/) | Gets and sets the display mode of the background |
|[GetShadow](./getshadow/) | True if the frame has a shadow. |
|[SetShadow](./setshadow/) | True if the frame has a shadow. |
|[GetShapeProperties](./getshapeproperties/) | Gets the ShapeProperties object. |
|[IsDefaultPosBeSet](./isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
|[GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Represents x of default position in units of Fraction of the chart area. |
|[GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Represents y of default position in units of Fraction of the chart area. |
|[GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Represents width of default position in units of Fraction of the chart area. |
|[GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Represents height of default position in units of Fraction of the chart area. |
|[GetBorder](./getborder/) | Gets the Line</see>. |
|[GetArea](./getarea/) | Gets the Area</see>. |
|[GetTextOptions](./gettextoptions/) | Gets and sets the options of the text. |
|[GetFont](./getfont/) | Gets a Font object of the specified ChartFrame object. |
|[GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[IsAutomaticSize](./isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
|[SetIsAutomaticSize](./setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
|[GetWidthRatioToChart](./getwidthratiotochart/) | Gets or sets the width of frame in units of ratio of the chart area. |
|[SetWidthRatioToChart](./setwidthratiotochart/) | Gets or sets the width of frame in units of ratio of the chart area. |
|[GetHeightRatioToChart](./getheightratiotochart/) | Gets or sets the height of frame in units of ratio of the chart area. |
|[SetHeightRatioToChart](./setheightratiotochart/) | Gets or sets the height of frame in units of ratio of the chart area. |
|[GetXPixel](./getxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
|[SetXPixel](./setxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
|[GetYPixel](./getypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
|[SetYPixel](./setypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
|[GetWidthPixel](./getwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
|[SetWidthPixel](./setwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
|[GetHeightPixel](./getheightpixel/) | Gets or sets the height of frame in units of Pixel. |
|[SetHeightPixel](./setheightpixel/) | Gets or sets the height of frame in units of Pixel. |
|[SetPositionAuto](./setpositionauto/) | Set position of the frame to automatic |
|[IsDeleted](./isdeleted/) | Indicates whether this data labels is deleted. |
|[SetIsDeleted](./setisdeleted/) | Indicates whether this data labels is deleted. |
|[GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
|[SetTextHorizontalAlignment](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
|[GetTextVerticalAlignment](./gettextverticalalignment/) | Gets or sets the text vertical alignment of text. |
|[SetTextVerticalAlignment](./settextverticalalignment/) | Gets or sets the text vertical alignment of text. |
|[GetRotationAngle](./getrotationangle/) | Represents text rotation angle. |
|[SetRotationAngle](./setrotationangle/) | Represents text rotation angle. |
|[IsAutomaticRotation](./isautomaticrotation/) | Indicates whether the text of the chart is automatically rotated. |
|[GetReadingOrder](./getreadingorder/) | Represents text reading order. |
|[SetReadingOrder](./setreadingorder/) | Represents text reading order. |
|[IsResizeShapeToFitText](./isresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting iswhen text within a shape is scaled in order to contain all the text inside. |
|[SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting iswhen text within a shape is scaled in order to contain all the text inside. |
|[IsAutoText](./isautotext/) | Indicates the text is auto generated. |
|[SetIsAutoText](./setisautotext/) | Indicates the text is auto generated. |
|[GetLinkedSource](./getlinkedsource/) | Gets and sets a reference to the worksheet. |
|[SetLinkedSource](./setlinkedsource/) | Gets and sets a reference to the worksheet. |
|[GetDirectionType](./getdirectiontype/) | Gets and sets the direction of text. |
|[SetDirectionType](./setdirectiontype/) | Gets and sets the direction of text. |
|[IsTextWrapped](./istextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
|[SetIsTextWrapped](./setistextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
