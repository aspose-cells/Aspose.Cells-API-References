---
title: Worksheet.IsProtected
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates if the worksheet is protected
type: docs
url: /net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Indicates if the worksheet is protected.

```csharp
public bool IsProtected { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].IsProtected);
[Test]
        public void Property_IsProtected()
        {
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "abcd");
            workbook.Worksheets[0].Protect(ProtectionType.All, "abcd", null);
            workbook.Save(Constants.destPath + "CELLSJAVA42568.ods");
            workbook.Save(Constants.destPath + "CELLSJAVA42568.xls");
            workbook.Save(Constants.destPath + "CELLSJAVA42568.xlsx");
            workbook.Save(Constants.destPath + "CELLSJAVA42568.xlsb");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42568.ods");
            Assert.IsTrue(workbook.Worksheets[0].IsProtected);
              workbook =  new Workbook(Constants.destPath + "CELLSJAVA42568.xls");
            Assert.IsTrue(workbook.Worksheets[0].IsProtected);
              workbook =  new Workbook(Constants.destPath + "CELLSJAVA42568.xlsx");
            Assert.IsTrue(workbook.Worksheets[0].IsProtected);
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42568.xlsb");
            Assert.IsTrue(workbook.Worksheets[0].IsProtected);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


