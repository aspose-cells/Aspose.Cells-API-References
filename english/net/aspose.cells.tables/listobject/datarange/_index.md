---
title: ListObject.DataRange
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the data range of the ListObject
type: docs
url: /net/aspose.cells.tables/listobject/datarange/
---
## ListObject.DataRange property

Gets the data range of the ListObject.

```csharp
public Range DataRange { get; }
```

### Examples

```csharp
// Called: range[i, loMain.DataRange.ColumnCount - 1].Formula = sFormula;
[Test]
        public void Property_DataRange()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Formula/N25574.xlsm");
            Worksheet worksheet = workbook.Worksheets[0];
            int tableIdx1 = worksheet.ListObjects.Add(1, 0, 6, 19, true);
            worksheet.ListObjects[tableIdx1].DisplayName = "Table1.name.";
            int tableIdx2 = worksheet.ListObjects.Add(9, 0, 13, 18, true);
            worksheet.ListObjects[tableIdx2].DisplayName = "Table2.name.";
            Aspose.Cells.Tables.ListObject loMain = worksheet.ListObjects[tableIdx1];
            String sFormula = "=IFERROR(VLOOKUP(Table1.name.[a],Table2.name.[[a]:[b]],2,FALSE),2)";
            Aspose.Cells.Range range = loMain.DataRange;
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, loMain.DataRange.ColumnCount - 1].Formula = sFormula;
            }
            Assert.AreEqual(range[0, loMain.DataRange.ColumnCount - 1].Formula, "=IFERROR(VLOOKUP([a],Table2.name.[[a]:[b]],2,FALSE),2)");
            workbook.CalculateFormula();
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


