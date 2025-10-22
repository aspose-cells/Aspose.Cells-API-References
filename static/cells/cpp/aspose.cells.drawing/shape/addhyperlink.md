##Aspose::Cells::Drawing::Shape::AddHyperlink method
'Aspose::Cells::Drawing::Shape::AddHyperlink method. Adds a hyperlink to the shape in C++.'
## Shape::AddHyperlink(const U16String\&) method
Adds a hyperlink to the shape.
```cpp
Hyperlink Aspose::Cells::Drawing::Shape::AddHyperlink(const U16String &address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| address | const U16String\& | Address of the hyperlink. |
## ReturnValue
Return the new hyperlink object.
## Examples
```cpp
U16String val = u"https://www.aspose.com/";
Hyperlink hyperlink = shape.AddHyperlink(val);
```
## See Also
* Class [Hyperlink](../../../aspose.cells/hyperlink/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::AddHyperlink(const char16_t*) method
Adds a hyperlink to the shape.
```cpp
Hyperlink Aspose::Cells::Drawing::Shape::AddHyperlink(const char16_t *address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| address | const char16_t* | Address of the hyperlink. |
## ReturnValue
Return the new hyperlink object.
## Examples
```cpp
Hyperlink hyperlink = shape.AddHyperlink(u"https://www.aspose.com/");
```
## See Also
* Class [Hyperlink](../../../aspose.cells/hyperlink/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
