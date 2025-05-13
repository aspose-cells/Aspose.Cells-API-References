---
title: Protection.AllowDeletingRow
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the deletion of rows is allowed on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Represents if the deletion of rows is allowed on a protected worksheet.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Remarks

The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

### Examples

```csharp
// Called: Assert.IsTrue(sheet.Protection.AllowDeletingRow);
public void Protection_Property_AllowDeletingRow()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xml");
    Worksheet sheet = workbook.Worksheets["Cars (1)"];
    Assert.IsTrue(sheet.Protection.AllowDeletingRow);
    Assert.IsTrue(sheet.Protection.AllowSorting);
    Assert.IsTrue(sheet.Protection.AllowFiltering);
    Assert.IsTrue(sheet.Protection.AllowFormattingColumn);
    workbook.Save(Constants.destPath + "example.xml");
    workbook = new Workbook(Constants.destPath + "example.xml");
    sheet = workbook.Worksheets["Cars (1)"];
    Assert.IsTrue(sheet.Protection.AllowDeletingRow);
    Assert.IsTrue(sheet.Protection.AllowSorting);
    Assert.IsTrue(sheet.Protection.AllowFiltering);
    Assert.IsTrue(sheet.Protection.AllowFormattingColumn);
}
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


