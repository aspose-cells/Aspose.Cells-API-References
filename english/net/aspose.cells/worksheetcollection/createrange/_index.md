---
title: WorksheetCollection.CreateRange
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Creates a Range object from an address of the range
type: docs
url: /net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Creates a [`Range`](../../range/) object from an address of the range.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Int32 | The sheet index. |

### Return Value

A [`Range`](../../range/) object

### Examples

```csharp
// Called: Aspose.Cells.Range source = t.Worksheets.CreateRange("A1:F10",0);
[Test]
        public void Method_Int32_()
        {
            var fileName = Constants.PivotTableSourcePath + "CELLSNET-57571.xlsx";
            Workbook t = new Workbook(fileName);
            t.Save(Constants.destPath + "CELLSNET57651.dif");
            var workbook = new Aspose.Cells.Workbook(Constants.destPath + "CELLSNET57651.dif");
            workbook.Save(Constants.destPath + "CELLSNET57651.xlsx");
            Aspose.Cells.Range source = t.Worksheets.CreateRange("A1:F10",0);
            Aspose.Cells.Range dest = workbook.Worksheets.CreateRange("A1:F10", 0);
            RangeUtil.Compare(source, dest,false);
        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


