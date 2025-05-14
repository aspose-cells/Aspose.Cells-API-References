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
public void Worksheet_Property_IsProtected()
{
    Workbook workbook = new Workbook();
    workbook.Protect(ProtectionType.All, "abcd");
    workbook.Worksheets[0].Protect(ProtectionType.All, "abcd", null);
    workbook.Save(Constants.destPath + "example.ods");
    workbook.Save(Constants.destPath + "example.xls");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.IsTrue(workbook.Worksheets[0].IsProtected);
      workbook =  new Workbook(Constants.destPath + "example.xls");
    Assert.IsTrue(workbook.Worksheets[0].IsProtected);
      workbook =  new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(workbook.Worksheets[0].IsProtected);
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.IsTrue(workbook.Worksheets[0].IsProtected);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


