---
title: Outline.SummaryRowBelow
second_title: Aspose.Cells for .NET API Reference
description: Outline property. Indicates if the summary row will be positioned below the detail rows in the outline
type: docs
url: /net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Indicates if the summary row will be positioned below the detail rows in the outline.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Examples

```csharp
// Called: worksheet.Outline.SummaryRowBelow = false;
[Test]
        public void Property_SummaryRowBelow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42803.xlsb&quot;);
            Worksheet worksheet = workbook.Worksheets[&quot;Validations&quot;];
            worksheet.Outline.SummaryRowBelow = false;
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42803.xlsb&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42803.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA42803.xlsb&quot;);
            Assert.IsFalse(workbook.Worksheets[&quot;Validations&quot;].Outline.SummaryRowBelow);
        }
```

### See Also

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


