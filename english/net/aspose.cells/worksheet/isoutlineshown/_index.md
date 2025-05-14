---
title: Worksheet.IsOutlineShown
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether to show outline
type: docs
url: /net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Indicates whether to show outline.

```csharp
public bool IsOutlineShown { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(v, workbook.Worksheets[0].IsOutlineShown);
private void Worksheet_Property_IsOutlineShown(bool v)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].IsOutlineShown = v;
            Assert.AreEqual(v,workbook.Worksheets[0].IsOutlineShown);
            workbook.Save(Constants.destPath + "dest.xlsx");
            workbook = new Workbook(Constants.destPath + "dest.xlsx");
            Assert.AreEqual(v, workbook.Worksheets[0].IsOutlineShown);
            workbook.Save(Constants.destPath + "dest.xls");
            workbook = new Workbook(Constants.destPath + "dest.xls");
            Assert.AreEqual(v, workbook.Worksheets[0].IsOutlineShown);
            workbook.Save(Constants.destPath + "dest.xlsb");
            workbook = new Workbook(Constants.destPath + "dest.xlsb");
            Assert.AreEqual(v, workbook.Worksheets[0].IsOutlineShown);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


