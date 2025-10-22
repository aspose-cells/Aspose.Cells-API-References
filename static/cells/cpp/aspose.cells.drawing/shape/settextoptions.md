##Aspose::Cells::Drawing::Shape::SetTextOptions method
'Aspose::Cells::Drawing::Shape::SetTextOptions method. Represents the text options of the shape in C++.'
## Shape::SetTextOptions method
Represents the text options of the shape.
```cpp
void Aspose::Cells::Drawing::Shape::SetTextOptions(const TextOptions &value)
```
## Examples
```cpp
TextOptions opt = shape.GetTextOptions();
opt.SetColor(Color{ 0xff, 0, 0, 0xff });
opt.SetSize(8);
shape.SetTextOptions(opt);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
