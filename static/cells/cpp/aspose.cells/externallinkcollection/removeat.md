##Aspose::Cells::ExternalLinkCollection::RemoveAt method
'Aspose::Cells::ExternalLinkCollection::RemoveAt method. Removes the specified external link from the workbook in C++.'
## ExternalLinkCollection::RemoveAt(int32_t) method
Removes the specified external link from the workbook.
```cpp
void Aspose::Cells::ExternalLinkCollection::RemoveAt(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | the index of the external link to be removed. |
## Remarks
When removing the external link, all formulas that reference to it will be removed too because the references become invalid.
## See Also
* Class [Vector](../../vector/)
* Class [ExternalLinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## ExternalLinkCollection::RemoveAt(int32_t, bool) method
Removes the specified external link from the workbook.
```cpp
void Aspose::Cells::ExternalLinkCollection::RemoveAt(int32_t index, bool updateReferencesAsLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | the index of the external link to be removed. |
| updateReferencesAsLocal | bool | Whether update all references of given external link to reference of current workbook itself. Check [Clear(bool)](../clear/) to get more details about this parameter. |
## See Also
* Class [Vector](../../vector/)
* Class [ExternalLinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
