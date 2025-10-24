##Aspose::Cells::Slicers::Slicer::GetPlacement method
'Aspose::Cells::Slicers::Slicer::GetPlacement method. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet in C++.'
## Slicer::GetPlacement method
Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.
```cpp
PlacementType Aspose::Cells::Slicers::Slicer::GetPlacement()
```
## Examples
```cpp
if (slicer.GetPlacement() != PlacementType::FreeFloating)
{
slicer.SetPlacement(PlacementType::FreeFloating);
}
```
## See Also
* Enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
