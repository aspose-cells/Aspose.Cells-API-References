##Aspose::Cells::Drawing::Shape::GetTextOptions method
'Aspose::Cells::Drawing::Shape::GetTextOptions method. Represents the text options of the shape in C++.'
## Shape::GetTextOptions method
Represents the text options of the shape.
```cpp
TextOptions Aspose::Cells::Drawing::Shape::GetTextOptions()
```
## Examples
```cpp
TextOptions opt = shape.GetTextOptions();
opt.SetColor(Color{ 0xff, 0, 0, 0xff });
opt.SetSize(8);
shape.SetTextOptions(opt);
```
## See Also
* Class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
