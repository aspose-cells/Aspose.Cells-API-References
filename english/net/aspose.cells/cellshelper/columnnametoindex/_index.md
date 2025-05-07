---
title: CellsHelper.ColumnNameToIndex
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets column index according to column name
type: docs
url: /net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Gets column index according to column name.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnName | String | Column name. |

### Return Value

Column index.

### Examples

```csharp
// Called: blockRange.MoveTo(7, CellsHelper.ColumnNameToIndex("H")); //moving to H8
[Test]
	    public void Method_String_()
	    {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45171.xlsx");
            Aspose.Cells.Range blockRange = workbook.Worksheets.GetRangeByName("range");
            blockRange.MoveTo(7, CellsHelper.ColumnNameToIndex("H")); //moving to H8 
            Assert.AreEqual(workbook.Worksheets.Names["firstrow"].RefersTo, "=Sheet1!$H$8:$J$8");
            Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "CellsNet45171.xlsx");
	    }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


