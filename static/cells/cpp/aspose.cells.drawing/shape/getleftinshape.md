##Aspose::Cells::Drawing::Shape::GetLeftInShape method
'Aspose::Cells::Drawing::Shape::GetLeftInShape method. Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape in C++.'
## Shape::GetLeftInShape method
Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.
```cpp
int32_t Aspose::Cells::Drawing::Shape::GetLeftInShape()
```
## Remarks
Only Applies when this shape in the group or chart.
## Examples
```cpp
if (shape.IsInGroup() && shape.GetLeftInShape() == 2000)
shape.SetLeftInShape(4000);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
