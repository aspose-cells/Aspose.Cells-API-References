---
title: Worksheet.Validations
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the data validation setting collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Gets the data validation setting collection in the worksheet.

```csharp
public ValidationCollection Validations { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("='Set Variables'!J$1:J$2",sheet.Validations[0].Formula1);
[Test]
        public void Property_Validations()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45858.xlsx");
            Worksheet sheet = workbook.Worksheets[11];
            Assert.AreEqual("='Set Variables'!J$1:J$2",sheet.Validations[0].Formula1);
            workbook.Save(Constants.destPath + "CellsNet45858.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet45858.xlsx");
            Assert.AreEqual("='Set Variables'!J$1:J$2", workbook.Worksheets[11].Validations[0].Formula1);
        }
```

### See Also

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


