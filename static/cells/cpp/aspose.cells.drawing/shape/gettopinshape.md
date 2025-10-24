##Aspose::Cells::Drawing::Shape::GetTopInShape method
'Aspose::Cells::Drawing::Shape::GetTopInShape method. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape in C++.'
## Shape::GetTopInShape method
Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.
```cpp
int32_t Aspose::Cells::Drawing::Shape::GetTopInShape()
```
## Remarks
Only Applies when this shape in the group or chart.
## Examples
```cpp
if (shape.IsInGroup() && shape.GetTopInShape() == 8000)
shape.SetTopInShape(4000);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
