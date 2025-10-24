##Aspose::Cells::Drawing::ShapeCollection::AddFreeFloatingShape method
'Aspose::Cells::Drawing::ShapeCollection::AddFreeFloatingShape method. Adds a free floating shape to the worksheet.Only applies for line/image shape in C++.'
## ShapeCollection::AddFreeFloatingShape method
Adds a free floating shape to the worksheet.Only applies for line/image shape.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddFreeFloatingShape(MsoDrawingType type, int32_t top, int32_t left, int32_t height, int32_t width, const Vector<uint8_t> &imageData, bool isOriginalSize)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The shape type. |
| top | int32_t | Represents the vertical offset of shape from the worksheet's top row, in unit of pixel. |
| left | int32_t | Represents the horizontal offset of shape from the worksheet's left column, in unit of pixel. |
| height | int32_t | Represents the height of [LineShape](../../lineshape/), in unit of pixel. |
| width | int32_t | Represents the width of [LineShape](../../lineshape/), in unit of pixel. |
| imageData | const Vector \<uint8_t\>\& | The image data,only applies for the picture. |
| isOriginalSize | bool | Whether the shape use original size if the shape is image. |
## ReturnValue
## Examples
```cpp
//add a line
Vector<uint8_t> lineImageData{ 0 };//Adding lines does not require image data(Note: You need to read the data into this variable.)
Shape floatingShape_Line = shapes.AddFreeFloatingShape(MsoDrawingType::Line, 100, 100, 100, 50, lineImageData, false);
//add a picture
Vector<uint8_t> imgData{ 0 };//Gets image data into 'imgData' from file(e.g image.jpg . Note: You need to read the data into this variable.).
Shape floatingShape_Picture = shapes.AddFreeFloatingShape(MsoDrawingType::Picture, 200, 100, 100, 50, imgData, false);
```
## See Also
* Class [Shape](../../shape/)
* Enum [MsoDrawingType](../../msodrawingtype/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
