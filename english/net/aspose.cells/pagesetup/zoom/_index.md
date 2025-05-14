---
title: PageSetup.Zoom
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the scaling factor in percent. It should be between 10 and 400
type: docs
url: /net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Represents the scaling factor in percent. It should be between 10 and 400.

```csharp
public int Zoom { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(x, workbook.Worksheets[0].PageSetup.Zoom);
public void PageSetup_Property_Zoom()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    int x = workbook.Worksheets[0].PageSetup.Zoom;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(x, workbook.Worksheets[0].PageSetup.Zoom);

}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


