##Aspose::Cells::Drawing::ShapeCollection::AddPictureInChart method
'Aspose::Cells::Drawing::ShapeCollection::AddPictureInChart method. Adds a picture to the chart in C++.'
## ShapeCollection::AddPictureInChart method
Adds a picture to the chart.
```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::ShapeCollection::AddPictureInChart(int32_t top, int32_t left, const Vector<uint8_t> &stream, int32_t widthScale, int32_t heightScale)
```
| Parameter | Type | Description |
| --- | --- | --- |
| top | int32_t | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | int32_t | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| stream | const Vector \<uint8_t\>\& | Stream object which contains the image data. |
| widthScale | int32_t | Scale of image width, a percentage. |
| heightScale | int32_t | Scale of image height, a percentage. |
## ReturnValue
Returns a [Picture](../../picture/) object.
## See Also
* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
