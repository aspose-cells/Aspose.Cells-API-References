##Aspose::Cells::Drawing::ShapeCollection::AddOleObject method
'Aspose::Cells::Drawing::ShapeCollection::AddOleObject method. Adds an OleObject in C++.'
## ShapeCollection::AddOleObject method
Adds an [OleObject](../../oleobject/).
```cpp
OleObject Aspose::Cells::Drawing::ShapeCollection::AddOleObject(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width, const Vector<uint8_t> &imageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t |  |
| top | int32_t |  |
| upperLeftColumn | int32_t |  |
| left | int32_t |  |
| height | int32_t |  |
| width | int32_t |  |
| imageData | const Vector \<uint8_t\>\& |  |
## ReturnValue
## Examples
```cpp
Vector<uint8_t> imgData{ 0 };//Gets image data into 'imgData' from file(e.g image.jpg . Note: You need to read the data into this variable.).
OleObject oleObject = shapes.AddOleObject(4, 0, 5, 0, 300, 500, imgData);
```
## See Also
* Class [OleObject](../../oleobject/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
