##Aspose::Cells::Drawing::ShapeCollection::Get method
'Aspose::Cells::Drawing::ShapeCollection::Get method. Gets the Shape object at the specific index in the list in C++.'
## ShapeCollection::Get(int32_t) method
Gets the [Shape](../../shape/) object at the specific index in the list.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index. |
## ReturnValue
## Examples
```cpp
//get the first shape
Shape shape = shapes.Get(0);
```
## See Also
* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::Get(const U16String\&) method
Gets the [Shape](../../shape/) object by the name of the shape.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(const U16String &name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | const U16String\& | The name of the shape. |
## ReturnValue
## Examples
```cpp
//add a shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//get the shape by the name.
U16String val = u"Rectangle 1";
Shape shape1 = shapes.Get(val);
if (!shape1.IsNull())
{
//Got the shape named 'Rectangle 1'.
}
```
## See Also
* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::Get(const char16_t*) method
Gets the [Shape](../../shape/) object by the name of the shape.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(const char16_t *name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | const char16_t* | The name of the shape. |
## ReturnValue
## Examples
```cpp
//add a shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//get the shape
Shape shape1 = shapes.Get(u"Rectangle 1");
if (!shape1.IsNull())
{
//Got the shape named 'Rectangle 1'.
}
```
## See Also
* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
