---
title: AutoFitterOptions.IgnoreHidden
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Ignores the hidden rows/columns
type: docs
url: /net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Ignores the hidden rows/columns.

```csharp
public bool IgnoreHidden { get; set; }
```

### Examples

```csharp
// Called: IgnoreHidden = true,
[Test]
	    public void Property_IgnoreHidden()
	    {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET45714.xlsx&quot;);
            Worksheet worksheet = wb.Worksheets[0];

            

            AutoFitterOptions AFOptions = new AutoFitterOptions()
            {
                OnlyAuto = true,
                IgnoreHidden = true,
                AutoFitMergedCells = true
            };
            worksheet.AutoFitRows(AFOptions);


            Assert.AreEqual(worksheet.Cells.GetRowHeight(0),30);
            Assert.AreEqual(worksheet.Cells.GetRowHeight(1), 15);
	    }
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


