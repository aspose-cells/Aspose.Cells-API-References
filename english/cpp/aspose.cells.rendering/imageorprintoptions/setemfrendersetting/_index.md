---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::SetEmfRenderSetting method
linktitle: SetEmfRenderSetting
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::SetEmfRenderSetting method. Setting for rendering Emf metafile in C++.'
type: docs
weight: 6600
url: /cpp/aspose.cells.rendering/imageorprintoptions/setemfrendersetting/
---
## ImageOrPrintOptions::SetEmfRenderSetting method


Setting for rendering Emf metafile.

```cpp
void Aspose::Cells::Rendering::ImageOrPrintOptions::SetEmfRenderSetting(EmfRenderSetting value)
```

## Remarks


EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../../../aspose.cells/emfrendersetting/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../../../aspose.cells/emfrendersetting/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
