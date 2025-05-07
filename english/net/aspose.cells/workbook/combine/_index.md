---
title: Workbook.Combine
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Combines another Workbook object
type: docs
url: /net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Combines another Workbook object.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | Workbook | Another Workbook object. |

### Remarks

Merge Excel, ODS , CSV and other files to one file.

### Examples

```csharp
// Called: worbook.Combine(worbook1);
[Test]
        public void Method_Workbook_()
        {
            Workbook worbook = new Workbook(Constants.sourcePath + "CellsNet44081.xlsx");
            Workbook worbook1 = new Workbook(Constants.sourcePath + "CellsNet44081.xlsx");
            worbook.Combine(worbook1);
            Assert.AreEqual("Sheet2", worbook.Worksheets[1].Name);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


