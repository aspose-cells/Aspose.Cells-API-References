##Aspose::Cells::Properties::BuiltInDocumentPropertyCollection::Get method
'Aspose::Cells::Properties::BuiltInDocumentPropertyCollection::Get method. Returns a DocumentProperty object by the name of the property in C++.'
## BuiltInDocumentPropertyCollection::Get(const U16String\&) method
Returns a [DocumentProperty](../../documentproperty/) object by the name of the property.
```cpp
DocumentProperty Aspose::Cells::Properties::BuiltInDocumentPropertyCollection::Get(const U16String &name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | const U16String\& | The case-insensitive name of the property to retrieve. |
## Remarks
The string names of the properties correspond to the names of the typed properties available from [BuiltInDocumentPropertyCollection](../).
If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new [DocumentProperty](../../documentproperty/) is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).
If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.
## See Also
* Class [DocumentProperty](../../documentproperty/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [BuiltInDocumentPropertyCollection](../)
* Namespace [Aspose::Cells::Properties](../../)
* Library [Aspose.Cells for C++](../../../)
## BuiltInDocumentPropertyCollection::Get(const char16_t*) method
Returns a [DocumentProperty](../../documentproperty/) object by the name of the property.
```cpp
DocumentProperty Aspose::Cells::Properties::BuiltInDocumentPropertyCollection::Get(const char16_t *name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | const char16_t* | The case-insensitive name of the property to retrieve. |
## Remarks
The string names of the properties correspond to the names of the typed properties available from [BuiltInDocumentPropertyCollection](../).
If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new [DocumentProperty](../../documentproperty/) is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).
If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.
## See Also
* Class [DocumentProperty](../../documentproperty/)
* Class [BuiltInDocumentPropertyCollection](../)
* Namespace [Aspose::Cells::Properties](../../)
* Library [Aspose.Cells for C++](../../../)
## BuiltInDocumentPropertyCollection::Get(int32_t) method
Returns a [DocumentProperty](../../documentproperty/) object by index.
```cpp
DocumentProperty Aspose::Cells::Properties::BuiltInDocumentPropertyCollection::Get(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | Zero-based index of the [DocumentProperty](../../documentproperty/) to retrieve. |
## See Also
* Class [DocumentProperty](../../documentproperty/)
* Class [BuiltInDocumentPropertyCollection](../)
* Namespace [Aspose::Cells::Properties](../../)
* Library [Aspose.Cells for C++](../../../)
