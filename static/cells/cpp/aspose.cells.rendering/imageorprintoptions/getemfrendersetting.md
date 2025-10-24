##Aspose::Cells::Rendering::ImageOrPrintOptions::GetEmfRenderSetting method
'Aspose::Cells::Rendering::ImageOrPrintOptions::GetEmfRenderSetting method. Setting for rendering Emf metafiles in source file in C++.'
## ImageOrPrintOptions::GetEmfRenderSetting method
Setting for rendering Emf metafiles in source file.
```cpp
EmfRenderSetting Aspose::Cells::Rendering::ImageOrPrintOptions::GetEmfRenderSetting()
```
## Remarks
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../../../aspose.cells/emfrendersetting/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../../../aspose.cells/emfrendersetting/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.
## See Also
* Enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
