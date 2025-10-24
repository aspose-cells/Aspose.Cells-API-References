##Aspose::Cells::Slicers::Slicer::SetAlternativeText method
'Aspose::Cells::Slicers::Slicer::SetAlternativeText method. Returns or sets the descriptive (alternative) text string of the Slicer object in C++.'
## Slicer::SetAlternativeText(const U16String\&) method
Returns or sets the descriptive (alternative) text string of the [Slicer](../) object.
```cpp
void Aspose::Cells::Slicers::Slicer::SetAlternativeText(const U16String &value)
```
## Examples
```cpp
U16String val = u"AlternativeText test";
if (slicer.GetAlternativeText().IsNull())
{
slicer.SetAlternativeText(val);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## Slicer::SetAlternativeText(const char16_t*) method
Returns or sets the descriptive (alternative) text string of the [Slicer](../) object.
```cpp
void Aspose::Cells::Slicers::Slicer::SetAlternativeText(const char16_t *value)
```
## Examples
```cpp
if (slicer.GetAlternativeText().IsNull())
{
slicer.SetAlternativeText(u"AlternativeText test");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
