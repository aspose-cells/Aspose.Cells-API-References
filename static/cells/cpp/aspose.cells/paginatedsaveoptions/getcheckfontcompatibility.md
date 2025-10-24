##Aspose::Cells::PaginatedSaveOptions::GetCheckFontCompatibility method
'Aspose::Cells::PaginatedSaveOptions::GetCheckFontCompatibility method. Indicates whether to check font compatibility for every character in text in C++.'
## PaginatedSaveOptions::GetCheckFontCompatibility method
Indicates whether to check font compatibility for every character in text.
```cpp
bool Aspose::Cells::PaginatedSaveOptions::GetCheckFontCompatibility()
```
## Remarks
The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;
## See Also
* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
