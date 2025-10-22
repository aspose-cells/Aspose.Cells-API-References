##Aspose::Cells::Drawing::ShapeCollection::Remove method
'Aspose::Cells::Drawing::ShapeCollection::Remove method. Remove the shape in C++.'
## ShapeCollection::Remove method
Remove the shape.
```cpp
void Aspose::Cells::Drawing::ShapeCollection::Remove(const Shape &shape)
```
| Parameter | Type | Description |
| --- | --- | --- |
| shape | const Shape\& |  |
## Examples
```cpp
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
//get the shape
Shape s = shapes.Get(u"Rectangle 1");// or shapes[0];
if (!s.IsNull())
{
//remove
shapes.Remove(s);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../../shape/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
