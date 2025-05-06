---
title: Workbook.CopyTheme
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Copies the theme from another workbook
type: docs
url: /net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Copies the theme from another workbook.

```csharp
public void CopyTheme(Workbook source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source workbook. |

### Examples

```csharp
// Called: nwb.CopyTheme(wb);
[Test]
        public void Method_Workbook_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41754.xlsx&quot;);
            Workbook nwb = new Workbook();
            nwb.Copy(wb);
            nwb.CopyTheme(wb);
            nwb.Save(Constants.destPath + &quot;dest.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;dest.xlsx&quot;);
            Assert.AreEqual(2, wb.Worksheets[0].Shapes.Count);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


