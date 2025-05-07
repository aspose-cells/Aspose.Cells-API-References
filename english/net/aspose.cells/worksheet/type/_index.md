---
title: Worksheet.Type
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents worksheet type
type: docs
url: /net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Represents worksheet type.

```csharp
public SheetType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Type, SheetType.Chart);
[Test]
        public void Property_Type()
        {
            var workbook = new Workbook(Constants.sourcePath + "CellsJava42923.xls");
            Assert.AreEqual(workbook.Worksheets[0].Type, SheetType.Chart);
            Assert.IsTrue(workbook.Worksheets[1].Charts[0].PageSetup.PrinterSettings == null);
            Assert.AreEqual(2, workbook.Worksheets[1].Charts.Count);
            workbook.Save(Constants.destPath + "CellsJava42923.xls");
        }
```

### See Also

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


