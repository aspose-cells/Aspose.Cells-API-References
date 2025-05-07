---
title: WorksheetCollection.Names
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the collection of all the Name objects in the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Gets the collection of all the Name objects in the spreadsheet.

```csharp
public NameCollection Names { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets.Names["YY"].RefersTo, "=Sheet3!$A$10:$L$16");
[Test]
        public void Property_Names()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestCellsNet16021.xls");
            Aspose.Cells.Range r1 = workbook.Worksheets.GetRangeByName("AA");

            r1.MoveTo(0, 0);

            Aspose.Cells.Range r2 = workbook.Worksheets.GetRangeByName("XX");

            r2.MoveTo(0, 0);

            Aspose.Cells.Range r3 = workbook.Worksheets.GetRangeByName("GG");

            r3.MoveTo(0, 0);


            Assert.AreEqual(workbook.Worksheets.Names["BB"].RefersTo, "=Sheet2!$D$10:$G$14");
            Assert.AreEqual(workbook.Worksheets.Names["YY"].RefersTo, "=Sheet3!$A$10:$L$16");
            Assert.AreEqual(workbook.Worksheets.Names["HH"].RefersTo, "=Sheet1!$G$7:$Q$12");
        }
```

### See Also

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


