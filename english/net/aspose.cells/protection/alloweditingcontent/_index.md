---
title: Protection.AllowEditingContent
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to edit contents of locked cells on a protected worksheet
type: docs
url: /net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Represents if the user is allowed to edit contents of locked cells on a protected worksheet.

```csharp
public bool AllowEditingContent { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(!workbook.Worksheets["Graph"].Protection.AllowEditingContent);
public void Protection_Property_AllowEditingContent()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsb");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(!workbook.Worksheets["Graph"].Protection.AllowEditingContent);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.IsTrue(!workbook.Worksheets["Graph"].Protection.AllowEditingContent);

}
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


