##Aspose::Cells::Drawing::TextBoxCollection::Get method
'Aspose::Cells::Drawing::TextBoxCollection::Get method. Gets the TextBox element at the specified index in C++.'
## TextBoxCollection::Get(int32_t) method
Gets the [TextBox](../../textbox/) element at the specified index.
```cpp
TextBox Aspose::Cells::Drawing::TextBoxCollection::Get(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The zero based index of the element. |
## ReturnValue
The element at the specified index.
## Examples
```cpp
int tbxTndex = textBoxCollection.GetCount() - 1;
TextBox txb = textBoxCollection.Get(tbxTndex);
```
## See Also
* Class [TextBox](../../textbox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [TextBoxCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## TextBoxCollection::Get(const U16String\&) method
Gets the [TextBox](../../textbox/) element by the name.
```cpp
TextBox Aspose::Cells::Drawing::TextBoxCollection::Get(const U16String &name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | const U16String\& | The name of the text box. |
## ReturnValue
## Examples
```cpp
U16String txtboxName = u"textbox 1";
TextBox txb2 = textBoxCollection.Get(txtboxName);
if (!txb2.IsNull())
{
//do what you want
}
```
## See Also
* Class [TextBox](../../textbox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [TextBoxCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## TextBoxCollection::Get(const char16_t*) method
Gets the [TextBox](../../textbox/) element by the name.
```cpp
TextBox Aspose::Cells::Drawing::TextBoxCollection::Get(const char16_t *name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | const char16_t* | The name of the text box. |
## ReturnValue
## Examples
```cpp
TextBox txb2 = textBoxCollection.Get(u"textbox 1");
if (!txb2.IsNull())
{
//do what you want
}
```
## See Also
* Class [TextBox](../../textbox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [TextBoxCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
