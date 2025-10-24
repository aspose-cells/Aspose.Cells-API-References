##Aspose::Cells::PaginatedSaveOptions::GetEmfRenderSetting method
'Aspose::Cells::PaginatedSaveOptions::GetEmfRenderSetting method. Setting for rendering Emf metafile in C++.'
## PaginatedSaveOptions::GetEmfRenderSetting method
Setting for rendering Emf metafile.
```cpp
EmfRenderSetting Aspose::Cells::PaginatedSaveOptions::GetEmfRenderSetting()
```
## Remarks
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../../emfrendersetting/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../../emfrendersetting/).
## See Also
* Enum [EmfRenderSetting](../../emfrendersetting/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
