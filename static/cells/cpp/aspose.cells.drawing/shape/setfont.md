##Aspose::Cells::Drawing::Shape::SetFont method
'Aspose::Cells::Drawing::Shape::SetFont method. Represents the font of shape in C++.'
## Shape::SetFont method
Represents the font of shape.
```cpp
void Aspose::Cells::Drawing::Shape::SetFont(const Aspose::Cells::Font &value)
```
## Examples
```cpp
Font font = shape.GetFont();
font.SetName(u"Arial");
font.SetSize(12);
font.SetColor(Color{ 0xff, 0xff, 0, 0 });
shape.SetFont(font);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Font](../../../aspose.cells/font/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
