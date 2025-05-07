---
title: PivotTable.GetChildren
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the Children Pivot Tables which use this PivotTable data as data source
type: docs
url: /net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

Gets the Children Pivot Tables which use this PivotTable data as data source.

```csharp
public PivotTable[] GetChildren()
```

### Return Value

the PivotTable array object

### Examples

```csharp
// Called: PivotTable[] tables = wb.Worksheets[0].PivotTables[0].GetChildren();
[Test]
        public void Method_GetChildren()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET45740_";
            Workbook wb = new Workbook(filePath + "Nested PivotTable.xlsx");
            PivotTable[] tables = wb.Worksheets[0].PivotTables[0].GetChildren();
            PivotTable[] tables2 = wb.Worksheets[0].PivotTables[1].GetChildren();
            Assert.AreEqual(tables.Length, 0);
            Assert.AreEqual(tables2.Length, 1);

        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


