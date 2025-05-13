---
title: PageSetup.Copy
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Copies the setting of the page setup
type: docs
url: /net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Copies the setting of the page setup.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | PageSetup | The source. |
| copyOptions | CopyOptions | The copy options. |

### Examples

```csharp
// Called: workbok.Worksheets[1].PageSetup.Copy(workbok.Worksheets[0].PageSetup,null);
public void PageSetup_Method_Copy()
{
    Workbook workbok = new Workbook();
    workbok.Worksheets.Add();
    workbok.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
    workbok.Worksheets[1].PageSetup.Copy(workbok.Worksheets[0].PageSetup,null);
    Assert.AreEqual(PaperSizeType.PaperA3, workbok.Worksheets[1].PageSetup.PaperSize);

}
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


