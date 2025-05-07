---
title: Worksheet.Cells
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the Cells collection
type: docs
url: /net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Gets the `Cells` collection.

```csharp
public Cells Cells { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells[0, 0].StringValue, "1,234.6");
[Test]
        public void Property_Cells()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41070/";
            Workbook workbook = new Workbook(filePath + "xls_export.html");
            Assert.AreEqual(workbook.Worksheets[0].Cells[0, 0].StringValue, "1,234.6");
        }
```

### See Also

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


