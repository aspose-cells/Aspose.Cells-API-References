##Aspose::Cells::Drawing::ShapeCollection::AddPicture method
'Aspose::Cells::Drawing::ShapeCollection::AddPicture method. Adds a picture to the collection in C++.'
## ShapeCollection::AddPicture(int32_t, int32_t, int32_t, int32_t, const Vector \<uint8_t\>\&) method
Adds a picture to the collection.
```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::ShapeCollection::AddPicture(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t lowerRightRow, int32_t lowerRightColumn, const Vector<uint8_t> &stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| upperLeftColumn | int32_t | Upper left column index. |
| lowerRightRow | int32_t | Lower right row index |
| lowerRightColumn | int32_t | Lower right column index |
| stream | const Vector \<uint8_t\>\& | Stream object which contains the image data. |
## ReturnValue
[Picture](../../picture/)[Picture](../../picture/) object.
## Examples
```cpp
//add a picture
Vector<uint8_t> fs{ 0 };//Gets image data into fs from file(e.g image.jpg . Note: You need to read the data into this variable.).
Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
```
## See Also
* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::AddPicture(int32_t, int32_t, const Vector \<uint8_t\>\&, int32_t, int32_t) method
Adds a picture to the collection.
```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::ShapeCollection::AddPicture(int32_t upperLeftRow, int32_t upperLeftColumn, const Vector<uint8_t> &stream, int32_t widthScale, int32_t heightScale)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| upperLeftColumn | int32_t | Upper left column index. |
| stream | const Vector \<uint8_t\>\& | Stream object which contains the image data. |
| widthScale | int32_t | Scale of image width, a percentage. |
| heightScale | int32_t | Scale of image height, a percentage. |
## ReturnValue
[Picture](../../picture/)[Picture](../../picture/) object.
## Examples
```cpp
//add a picture
Vector<uint8_t> fs{ 0 };//Gets image data into fs from file(e.g image.jpg . Note: You need to read the data into this variable.).
Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
```
## See Also
* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
