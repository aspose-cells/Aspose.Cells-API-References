---
title: Workbook.Combine
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Combines another Workbook object
type: docs
url: /net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Combines another Workbook object.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | Workbook | Another Workbook object. |

### Remarks

Merge Excel, ODS , CSV and other files to one file.

### Examples

```csharp
// Called: new Workbook(FileFormatType.Xlsx).Combine(wb); //should not cause exception
public void Workbook_Method_Combine()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xls");
    new Workbook(FileFormatType.Xlsx).Combine(wb); //should not cause exception
    wb = new Workbook(Constants.sourcePath + "example.xls");
    new Workbook(FileFormatType.Xlsx).Combine(wb); //should not cause exception
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


