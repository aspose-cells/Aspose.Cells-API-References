---
title: PivotField.CurrentPageItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the current page item showing for the page field valid only for page fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Represents the current page item showing for the page field (valid only for page fields).

```csharp
public short CurrentPageItem { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);
public void PivotField_Property_CurrentPageItem()
{
    string filePath = Constants.PivotTableSourcePath + @"NET43473and43474and43475_";
    var workbook = new Workbook(filePath + "source.xlsx");
    Console.WriteLine("source file=========");
    PivotFieldCollection pages = workbook.Worksheets[0].PivotTables[0].PageFields;
    Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);
    pages = workbook.Worksheets[1].PivotTables[0].PageFields;
    Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);

    RunReport(workbook);

    Console.WriteLine("after changing ========");
    pages = workbook.Worksheets[0].PivotTables[0].PageFields;
    Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);
    pages = workbook.Worksheets[1].PivotTables[0].PageFields;
    Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);

    workbook.Save(Constants.PivotTableDestPath + @"example.xlsx");
    workbook.Save(Constants.PivotTableDestPath + @"example.html", new HtmlSaveOptions());

    Workbook wb = new Workbook(filePath + "expected.xlsx");

    Console.WriteLine("expected file======");
    pages = wb.Worksheets[0].PivotTables[0].PageFields;
    Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);
    pages = wb.Worksheets[1].PivotTables[0].PageFields;
    Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


