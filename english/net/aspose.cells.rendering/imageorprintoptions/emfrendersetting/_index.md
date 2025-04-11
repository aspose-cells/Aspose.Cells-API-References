---
title: ImageOrPrintOptions.EmfRenderSetting
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Setting for rendering Emf metafiles in source file
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Setting for rendering Emf metafiles in source file.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Remarks

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfPlusPrefer is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is EmfOnly. For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### See Also

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


