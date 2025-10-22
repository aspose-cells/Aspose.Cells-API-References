##Aspose::Cells::Drawing::Shape::GetFont method
'Aspose::Cells::Drawing::Shape::GetFont method. Represents the font of shape in C++.'
## Shape::GetFont method
Represents the font of shape.
```cpp
Aspose::Cells::Font Aspose::Cells::Drawing::Shape::GetFont()
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
* Class [Font](../../../aspose.cells/font/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
