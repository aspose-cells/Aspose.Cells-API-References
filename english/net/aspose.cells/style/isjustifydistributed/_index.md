---
title: Style.IsJustifyDistributed
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates if the cells justified or distributed alignment should be used on the last line of text
type: docs
url: /net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Indicates if the cells justified or distributed alignment should be used on the last line of text.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Remarks

This is typical for East Asian alignments but not typical in other contexts.

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells["B3"].GetStyle().IsJustifyDistributed);
[Test]
        public void Property_IsJustifyDistributed()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet53111.xlsx");
            workbook.Save(Constants.destPath + "CellsNet53111.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet53111.xls");
            Assert.IsTrue(workbook.Worksheets[0].Cells["B3"].GetStyle().IsJustifyDistributed);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


