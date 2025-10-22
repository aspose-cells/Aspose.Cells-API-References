##Slicer Class
'Slicer class. Encapsulates the object that represents slicer in Go.'
## Slicer class
summary description of Slicer View
```go
type Slicer struct  {
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
|[AddPivotConnection](./addpivotconnection/) | Adds PivotTable connection. |
|[RemovePivotConnection](./removepivotconnection/) | Removes PivotTable connection. |
|[GetTitle](./gettitle/) | Specifies the title of the current Slicer object. |
|[SetTitle](./settitle/) | Specifies the title of the current Slicer object. |
|[GetAlternativeText](./getalternativetext/) | Returns or sets the descriptive (alternative) text string of the Slicer object. |
|[SetAlternativeText](./setalternativetext/) | Returns or sets the descriptive (alternative) text string of the Slicer object. |
|[IsPrintable](./isprintable/) | Indicates whether the slicer object is printable. |
|[SetIsPrintable](./setisprintable/) | Indicates whether the slicer object is printable. |
|[IsLocked](./islocked/) | Indicates whether the slicer shape is locked. |
|[SetIsLocked](./setislocked/) | Indicates whether the slicer shape is locked. |
|[GetPlacement](./getplacement/) | Represents the way the drawing object is attached to the cells below it.The property controls the placement of an object on a worksheet. |
|[SetPlacement](./setplacement/) | Represents the way the drawing object is attached to the cells below it.The property controls the placement of an object on a worksheet. |
|[GetLockedAspectRatio](./getlockedaspectratio/) | Indicates whether locking aspect ratio. |
|[SetLockedAspectRatio](./setlockedaspectratio/) | Indicates whether locking aspect ratio. |
|[GetLockedPosition](./getlockedposition/) | Indicates whether the specified slicer can be moved or resized by using the user interface. |
|[SetLockedPosition](./setlockedposition/) | Indicates whether the specified slicer can be moved or resized by using the user interface. |
|[Refresh](./refresh/) | Refreshing the slicer.Meanwhile, Refreshing and Calculating  relative PivotTables. |
|[GetShape](./getshape/) | Returns the Shape object associated with the specified slicer. Read-only. |
|[GetSlicerCache](./getslicercache/) | Returns the SlicerCache object associated with the slicer. Read-only. |
|[GetParent](./getparent/) | Returns the Worksheet object which contains this slicer. Read-only. |
|[GetStyleType](./getstyletype/) | Specify the type of Built-in slicer stylethe default type is SlicerStyleLight1 |
|[SetStyleType](./setstyletype/) | Specify the type of Built-in slicer stylethe default type is SlicerStyleLight1 |
|[GetName](./getname/) | Returns or sets the name of the specified slicer |
|[SetName](./setname/) | Returns or sets the name of the specified slicer |
|[GetCaption](./getcaption/) | Returns or sets the caption of the specified slicer. |
|[SetCaption](./setcaption/) | Returns or sets the caption of the specified slicer. |
|[GetCaptionVisible](./getcaptionvisible/) | Returns or sets whether the header that displays the slicer Caption is visiblethe default value is true |
|[SetCaptionVisible](./setcaptionvisible/) | Returns or sets whether the header that displays the slicer Caption is visiblethe default value is true |
|[GetNumberOfColumns](./getnumberofcolumns/) | Returns or sets the number of columns in the specified slicer. |
|[SetNumberOfColumns](./setnumberofcolumns/) | Returns or sets the number of columns in the specified slicer. |
|[GetColumnWidthPixel](./getcolumnwidthpixel/) | Gets or sets the width of each column in the slicer, in unit of pixels. |
|[SetColumnWidthPixel](./setcolumnwidthpixel/) | Gets or sets the width of each column in the slicer, in unit of pixels. |
|[GetColumnWidth](./getcolumnwidth/) | Returns or sets the width, in points, of each column in the slicer. |
|[SetColumnWidth](./setcolumnwidth/) | Returns or sets the width, in points, of each column in the slicer. |
|[GetRowHeightPixel](./getrowheightpixel/) | Returns or sets the height, in pixels, of each row in the specified slicer. |
|[SetRowHeightPixel](./setrowheightpixel/) | Returns or sets the height, in pixels, of each row in the specified slicer. |
|[GetRowHeight](./getrowheight/) | Returns or sets the height, in points, of each row in the specified slicer. |
|[SetRowHeight](./setrowheight/) | Returns or sets the height, in points, of each row in the specified slicer. |
