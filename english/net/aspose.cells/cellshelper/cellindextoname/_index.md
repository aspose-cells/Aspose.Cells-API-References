---
title: CellsHelper.CellIndexToName
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets cell name according to its row and column indexes
type: docs
url: /net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Gets cell name according to its row and column indexes.

```csharp
public static string CellIndexToName(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| column | Int32 | Column index. |

### Return Value

Name of cell.

### Examples

```csharp
// Called: Assert.AreEqual("=[na.xlsx]" + worksheet.Name + "!" + CellsHelper.CellIndexToName(1, 1),cell.Formula);
[Test]
	    public void Method_Int32_()
	    {
            Workbook one = new Workbook();
            WorksheetCollection worksheets = one.Worksheets;
            Worksheet worksheet = worksheets[0];
            Cell cell = worksheet.Cells[1, 1];
	        string f = "=[na.xlsx]" + worksheet.Name + "!" + CellsHelper.CellIndexToName(1, 1);
	        cell.Formula = f;
            Console.WriteLine(cell.Formula,f);
            worksheets.Add();
            worksheet = worksheets[1];
            cell = worksheet.Cells[1, 1];
            f = ("=[na.xlsx]" + worksheet.Name + "!" + CellsHelper.CellIndexToName(1, 1));
	        cell.Formula = f;
            Assert.AreEqual("=[na.xlsx]" + worksheet.Name + "!" + CellsHelper.CellIndexToName(1, 1),cell.Formula);
            one = Util.ReSave(one, SaveFormat.Xlsx);
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


