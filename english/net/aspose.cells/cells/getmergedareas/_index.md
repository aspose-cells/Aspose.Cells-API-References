---
title: Cells.GetMergedAreas
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets all merged cells
type: docs
url: /net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Gets all merged cells.

```csharp
public CellArea[] GetMergedAreas()
```

### Examples

```csharp
// Called: Assert.AreEqual(2, worksheet.Cells.GetMergedAreas().Length);
[Test]
        public void Method_GetMergedAreas()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CellsNet53994.xlsx");
            var worksheet = wb.Worksheets[0];
            var pivotTable = worksheet.PivotTables[0];
            var field = pivotTable.ColumnFields[1];

            foreach (PivotItem item in field.PivotItems)
            {
                item.IsHidden = item.Name != "债券借贷";
            }

            // 抛出错误 Aspose.Cells.CellsException:“Cells in range D2:D3 cannot be merged because cells in range B2:H2 have already been merged.”
            worksheet.RefreshPivotTables();
            Assert.AreEqual(2, worksheet.Cells.GetMergedAreas().Length);
            Assert.IsFalse(worksheet.Cells["B2"].IsMerged);
            Assert.IsTrue(worksheet.Cells["D2"].IsMerged);
            wb.Save(Constants.PivotTableDestPath + "CellsNet53994.xlsx");
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


