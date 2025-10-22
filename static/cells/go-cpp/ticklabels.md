##TickLabels Class
'TickLabels class. Encapsulates the object that represents ticklabels in Go.'
## TickLabels class
Represents the tick-mark labels associated with tick marks on a chart axis.
```go
type TickLabels struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetFont](./getfont/) | Returns a Font object that represents the font of the specified TickLabels object. |
|[GetAutoScaleFont](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[SetAutoScaleFont](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
|[GetBackgroundMode](./getbackgroundmode/) | Gets and sets the display mode of the background |
|[SetBackgroundMode](./setbackgroundmode/) | Gets and sets the display mode of the background |
|[GetRotationAngle](./getrotationangle/) | Represents text rotation angle in clockwise. |
|[SetRotationAngle](./setrotationangle/) | Represents text rotation angle in clockwise. |
|[IsAutomaticRotation](./isautomaticrotation/) | Indicates whether the rotation angle is automatic |
|[SetIsAutomaticRotation](./setisautomaticrotation/) | Indicates whether the rotation angle is automatic |
|[Get_NumberFormat](./get_numberformat/) | Represents the format string for the TickLabels object. |
|[SetNumberFormat](./setnumberformat/) | Represents the format string for the TickLabels object. |
|[GetNumber](./getnumber/) | Represents the format number for the TickLabels object. |
|[SetNumber](./setnumber/) | Represents the format number for the TickLabels object. |
|[GetNumberFormatLinked](./getnumberformatlinked/) | True if the number format is linked to the cells(so that the number format changes in the labels when it changes in the cells). |
|[SetNumberFormatLinked](./setnumberformatlinked/) | True if the number format is linked to the cells(so that the number format changes in the labels when it changes in the cells). |
|[GetDisplayNumberFormat](./getdisplaynumberformat/) | Gets and sets the display number format of tick labels. |
|[GetOffset](./getoffset/) | Gets and sets the distance of labels from the category axis.Only for category (x) axis. |
|[SetOffset](./setoffset/) | Gets and sets the distance of labels from the category axis.Only for category (x) axis. |
|[GetReadingOrder](./getreadingorder/) | Represents text reading order. |
|[SetReadingOrder](./setreadingorder/) | Represents text reading order. |
|[GetDirectionType](./getdirectiontype/) | Gets and sets the direction of text. |
|[SetDirectionType](./setdirectiontype/) | Gets and sets the direction of text. |
|[GetTickLabelItems](./getticklabelitems/) | Gets the display tick labels of the axis. |
|[GetAlignmentType](./getalignmenttype/) | Gets and sets the text alignment for the tick labels on the axis. |
|[SetAlignmentType](./setalignmenttype/) | Gets and sets the text alignment for the tick labels on the axis. |
