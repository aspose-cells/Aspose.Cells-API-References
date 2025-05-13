---
title: Worksheet.PageSetup
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents the page setup description in this sheet
type: docs
url: /net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Represents the page setup description in this sheet.

```csharp
public PageSetup PageSetup { get; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].PageSetup.PrintArea = "A1:L50";
public void Worksheet_Property_PageSetup()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].PageSetup.PrintArea = "A1:L50";
    workbook.Worksheets[0].PageSetup.PrintTitleRows = "1:2";
    workbook.Worksheets[0].PageSetup.PrintTitleColumns = "A:B";
    workbook.Worksheets[0].AutoFilter.Range = "A1:D1";
    workbook.Save(Constants.destPath + "TestPrintArea.xls");
    workbook = new Workbook(Constants.destPath + "TestPrintArea.xls");
    CheckTestPrintArea(workbook);
    workbook.Save(Constants.destPath + "TestPrintArea.xlsx");
    workbook = new Workbook(Constants.destPath + "TestPrintArea.xlsx");
    CheckTestPrintArea(workbook);
    workbook.Save(Constants.destPath + "TestPrintArea.xml");
    workbook = new Workbook(Constants.destPath + "TestPrintArea.xml");
    CheckTestPrintArea(workbook);
    workbook.Save(Constants.destPath + "TestPrintArea.ods");
    workbook = new Workbook(Constants.destPath + "TestPrintArea.ods");
    CheckTestPrintArea(workbook);
}
```

### See Also

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


