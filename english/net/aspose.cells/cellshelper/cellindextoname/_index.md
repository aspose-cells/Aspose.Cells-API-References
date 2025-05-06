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
// Called: CellsHelper.CellIndexToName(row: sourceSheet.Cells.MaxDataRow, column: sourceSheet.Cells.MaxDataColumn));
[Test]
        public void Method_Int32_()
        {
            string filePath = Constants.PivotTableSourcePath;
            var workbook = new Workbook();
            var sourceSheet = CreateSourceSheet44044(workbook);
            string source = string.Format(
                    &quot;=&apos;{0}&apos;!A1:{1}&quot;,
                    sourceSheet.Name,
                    CellsHelper.CellIndexToName(row: sourceSheet.Cells.MaxDataRow, column: sourceSheet.Cells.MaxDataColumn));
            CreatePivotSheet44044(
                workbook: workbook,
                sourceData: source);

            
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


