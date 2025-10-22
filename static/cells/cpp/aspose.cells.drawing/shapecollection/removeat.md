##Aspose::Cells::Drawing::ShapeCollection::RemoveAt method
'Aspose::Cells::Drawing::ShapeCollection::RemoveAt method. Remove the shape in C++.'
## ShapeCollection::RemoveAt method
Remove the shape.
```cpp
void Aspose::Cells::Drawing::ShapeCollection::RemoveAt(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index of the shape. |
## Examples
```cpp
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
//remove
shapes.RemoveAt(0);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
