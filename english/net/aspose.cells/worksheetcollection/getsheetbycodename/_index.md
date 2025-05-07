---
title: WorksheetCollection.GetSheetByCodeName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets the worksheet by the code name
type: docs
url: /net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Gets the worksheet by the code name.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| codeName | String | Worksheet code name. |

### Return Value

The element with the specified code name.

### Examples

```csharp
// Called: var ProblemSheet = ToTest.Worksheets.GetSheetByCodeName("Sheet5");
[Test]
        public void Method_String_()
        {
            Workbook ToTest = new Workbook(Constants.sourcePath + "Cellsnet44750.xls");
            var ProblemSheet = ToTest.Worksheets.GetSheetByCodeName("Sheet5");
            Assert.AreEqual(ProblemSheet.Shapes.Count, 0);
            ProblemSheet.Cells.DeleteColumn(0);
            var Renderer = new SheetRender(ProblemSheet, new ImageOrPrintOptions()); //Invalid Column Index
            Console.WriteLine(Renderer.PageCount);
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


