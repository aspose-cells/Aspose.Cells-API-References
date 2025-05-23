---
title: Worksheet.TabId
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Specifies the internal identifier for the sheet
type: docs
url: /net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Specifies the internal identifier for the sheet.

```csharp
public int TabId { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].TabId = 107;
public void Worksheet_Property_TabId()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].TabId = 107;
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.AreEqual(  workbook.Worksheets[0].TabId , 107);

}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


