##Aspose::Cells::Drawing::ShapePath::ArcTo method
'Aspose::Cells::Drawing::ShapePath::ArcTo method. Appends an elliptical arc to the current figure. The starting point is the end point of the current figure in C++.'
## ShapePath::ArcTo method
Appends an elliptical arc to the current figure. The starting point is the end point of the current figure.
```cpp
void Aspose::Cells::Drawing::ShapePath::ArcTo(float wR, float hR, float stAng, float swAng)
```
| Parameter | Type | Description |
| --- | --- | --- |
| wR | float | The half-width of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| hR | float | The half-height of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| stAng | float | The starting angle of the arc, measured in degrees clockwise from the x-axis(Unit: Degree). This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path. |
| swAng | float | The swing angle for an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.(Unit: Degree) |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapePath](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
