---
title: Worksheet.Outline
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the outline on this worksheet
type: docs
url: /net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Gets the outline on this worksheet.

```csharp
public Outline Outline { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets["Validations"].Outline.SummaryRowBelow);
[Test]
        public void Property_Outline()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42803.xlsb");
            Worksheet worksheet = workbook.Worksheets["Validations"];
            worksheet.Outline.SummaryRowBelow = false;
            workbook.Save(Constants.destPath + "CELLSJAVA42803.xlsb");
            workbook.Save(Constants.destPath + "CELLSJAVA42803.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42803.xlsb");
            Assert.IsFalse(workbook.Worksheets["Validations"].Outline.SummaryRowBelow);
        }
```

### See Also

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


