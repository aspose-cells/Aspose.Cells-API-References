---
title: Aspose::Cells::PaginatedSaveOptions::SetEmfRenderSetting method
linktitle: SetEmfRenderSetting
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetEmfRenderSetting method. Setting for rendering Emf metafile in C++.'
type: docs
weight: 4300
url: /cpp/aspose.cells/paginatedsaveoptions/setemfrendersetting/
---
## PaginatedSaveOptions::SetEmfRenderSetting method


Setting for rendering Emf metafile.

```cpp
void Aspose::Cells::PaginatedSaveOptions::SetEmfRenderSetting(EmfRenderSetting value)
```

## Remarks


EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../../emfrendersetting/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../../emfrendersetting/). 
## See Also

* Class [Vector](../../vector/)
* Enum [EmfRenderSetting](../../emfrendersetting/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
