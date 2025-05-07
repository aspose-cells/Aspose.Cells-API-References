---
title: PivotTable.PageFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as page fields
type: docs
url: /net/aspose.cells.pivot/pivottable/pagefields/
---
## PivotTable.PageFields property

Returns a PivotFields object that are currently shown as page fields.

```csharp
public PivotFieldCollection PageFields { get; }
```

### Examples

```csharp
// Called: pages = workbook.Worksheets[0].PivotTables[0].PageFields;
[Test]
        public void Property_PageFields()
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

            workbook.Save(Constants.PivotTableDestPath + @"NET43473and43474and43475.xlsx");
            workbook.Save(Constants.PivotTableDestPath + @"html/NET43473and43474and43475.html", new HtmlSaveOptions());

            Workbook wb = new Workbook(filePath + "expected.xlsx");

            Console.WriteLine("expected file======");
            pages = wb.Worksheets[0].PivotTables[0].PageFields;
            Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);
            pages = wb.Worksheets[1].PivotTables[0].PageFields;
            Console.WriteLine(pages[0].CurrentPageItem + "   " + pages[1].CurrentPageItem);
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


