---
title: PageSetup.Order
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the order that Microsoft Excel uses to number pages when printing a large worksheet
type: docs
url: /net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.

```csharp
public PrintOrderType Order { get; set; }
```

### Examples

```csharp
// Called: sheet.PageSetup.Order = PrintOrderType.DownThenOver;
public void PageSetup_Property_Order()
{
    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    sheet.PageSetup.Order = PrintOrderType.DownThenOver;

    checkPrintOrderType_DownThenOver(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkPrintOrderType_DownThenOver(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkPrintOrderType_DownThenOver(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    checkPrintOrderType_DownThenOver(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


