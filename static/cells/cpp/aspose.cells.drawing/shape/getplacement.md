##Aspose::Cells::Drawing::Shape::GetPlacement method
'Aspose::Cells::Drawing::Shape::GetPlacement method. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet in C++.'
## Shape::GetPlacement method
Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.
```cpp
PlacementType Aspose::Cells::Drawing::Shape::GetPlacement()
```
## Examples
```cpp
if (shape.GetPlacement() == PlacementType::Move)
shape.SetPlacement(PlacementType::MoveAndSize);
```
## See Also
* Enum [PlacementType](../../placementtype/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
