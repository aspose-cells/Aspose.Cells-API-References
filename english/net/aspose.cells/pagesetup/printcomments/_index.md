---
title: PageSetup.PrintComments
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the way comments are printed with the sheet
type: docs
url: /net/aspose.cells/pagesetup/printcomments/
---
## PageSetup.PrintComments property

Represents the way comments are printed with the sheet.

```csharp
public PrintCommentsType PrintComments { get; set; }
```

### Examples

```csharp
// Called: sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
public void PageSetup_Property_PrintComments()
{
    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;

    checkPrintCommentsType_PrintNoComments(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkPrintCommentsType_PrintNoComments(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkPrintCommentsType_PrintNoComments(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    checkPrintCommentsType_PrintNoComments(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


