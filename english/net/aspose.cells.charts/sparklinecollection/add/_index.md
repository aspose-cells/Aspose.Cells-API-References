---
title: SparklineCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SparklineCollection method. Add a sparkline
type: docs
url: /net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Add a sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline. |
| row | Int32 | The row index of the location. |
| column | Int32 | The column index of the location. |

### Examples

```csharp
// Called: workbook.Worksheets[0].SparklineGroups[0].SparklineCollection.Add("E6:P6", 5, 16);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava41096.xlsx");
            workbook.Worksheets[0].SparklineGroups[0].SparklineCollection.Add("E6:P6", 5, 16);
            workbook.Save(Constants.destPath + "CellsJava41096.xlsx");
        }
```

### See Also

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


