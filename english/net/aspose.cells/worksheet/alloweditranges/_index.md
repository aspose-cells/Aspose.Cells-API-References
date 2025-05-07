---
title: Worksheet.AllowEditRanges
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the allow edit range collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Gets the allow edit range collection in the worksheet.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[0].AllowEditRanges.Count, 2);
[Test]
        public void Property_AllowEditRanges()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA42534.xls");
            Assert.AreEqual(wb.Worksheets[0].AllowEditRanges.Count, 2);
            wb.Save(Constants.destPath + "CELLSJAVA42534.xlsb");
            wb = new Aspose.Cells.Workbook(Constants.destPath + "CELLSJAVA42534.xlsb");
            Assert.AreEqual(wb.Worksheets[0].AllowEditRanges.Count, 2);
            wb.Save(Constants.destPath + "CELLSJAVA42534.xlsx");
            wb = new Aspose.Cells.Workbook(Constants.destPath + "CELLSJAVA42534.xlsx");
            Assert.AreEqual(wb.Worksheets[0].AllowEditRanges.Count, 2);
            wb.Save(Constants.destPath + "CELLSJAVA42534.xlsb");
        }
```

### See Also

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


