##Aspose::Cells::Drawing::TextBoxCollection::Add method
'Aspose::Cells::Drawing::TextBoxCollection::Add method. Adds a textbox to the collection in C++.'
## TextBoxCollection::Add method
Adds a textbox to the collection.
```cpp
int32_t Aspose::Cells::Drawing::TextBoxCollection::Add(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| upperLeftColumn | int32_t | Upper left column index. |
| height | int32_t | Height of textbox, in unit of pixel. |
| width | int32_t | Width of textbox, in unit of pixel. |
## ReturnValue
[TextBox](../../textbox/) object index.
## Examples
```cpp
//add a TextBox
int index2 = textBoxCollection.Add(1, 1, 50, 100);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [TextBoxCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
