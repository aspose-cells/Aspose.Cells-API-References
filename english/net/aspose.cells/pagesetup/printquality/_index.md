---
title: PageSetup.PrintQuality
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the print quality
type: docs
url: /net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Represents the print quality.

```csharp
public int PrintQuality { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[1].PageSetup.PrintQuality, 144);
    public void PageSetup_Property_PrintQuality()            
    {
        Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
        for (int i = 0; i < workbook.Worksheets.Count; i++)
        {
            workbook.Worksheets[i].PageSetup.PrintQuality = 144;
        }
        workbook.Save(Constants.destPath + "example.xls");
        workbook = new Workbook(Constants.destPath + "example.xls");
        Assert.AreEqual(workbook.Worksheets[1].PageSetup.PrintQuality, 144);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


