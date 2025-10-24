##Aspose::Cells::Slicers::Slicer::SetTitle method
'Aspose::Cells::Slicers::Slicer::SetTitle method. Specifies the title of the current Slicer object in C++.'
## Slicer::SetTitle(const U16String\&) method
Specifies the title of the current [Slicer](../) object.
```cpp
void Aspose::Cells::Slicers::Slicer::SetTitle(const U16String &value)
```
## Examples
```cpp
U16String val = u"slicer title";
if(slicer.GetTitle().IsNull())
{
slicer.SetTitle(val);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## Slicer::SetTitle(const char16_t*) method
Specifies the title of the current [Slicer](../) object.
```cpp
void Aspose::Cells::Slicers::Slicer::SetTitle(const char16_t *value)
```
## Examples
```cpp
if (slicer.GetTitle().IsNull())
{
slicer.SetTitle(u"slicer title");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
