---
title: Workbook.RemovePersonalInformation
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Removes personal information
type: docs
url: /net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Removes personal information.

```csharp
public void RemovePersonalInformation()
```

### Examples

```csharp
// Called: wb.RemovePersonalInformation();
public void Workbook_Method_RemovePersonalInformation()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.IsTrue(wb.Settings.RemovePersonalInformation);
    wb.RemovePersonalInformation();
    // Save the Excel file.
    wb.Save(Constants.destPath + "example.xlsx", SaveFormat.Xlsx);
    wb = new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(wb.Worksheets[0].Comments[1].Note.Contains("Author"));
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


