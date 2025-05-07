---
title: PivotTable.ShowRowGrandTotals
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether to show grand totals for rows of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/showrowgrandtotals/
---
## PivotTable.ShowRowGrandTotals property

Indicates whether to show grand totals for rows of the pivot table.

```csharp
public bool ShowRowGrandTotals { get; set; }
```

### Examples

```csharp
// Called: pivotTable.ShowRowGrandTotals = true;
[Test]
        public void Property_ShowRowGrandTotals()
        {
            //Instantiating an Workbook object
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "Test_165529.xls");
            //Obtaining the reference of the newly added worksheet
            Worksheet sheet = workbook.Worksheets[workbook.Worksheets.Add()];
            //If I use this line, it works fine.
            //Worksheet sheet = workbook.Worksheets["Raw Data 2"];
            Cells cells = sheet.Cells;

            PivotTableCollection pivotTables = sheet.PivotTables;
            //Adding a PivotTable to the worksheet
            int index = pivotTables.Add("='Raw Data 2'!all", "G3", "PivotTable2");
            //Accessing the instance of the newly added PivotTable
            PivotTable pivotTable = pivotTables[index];
            pivotTable.ShowRowGrandTotals = true;
            pivotTable.ShowColumnGrandTotals = true;
            //Draging the second field to the row area.
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            //Draging the third field to the column area.
            pivotTable.AddFieldToArea(PivotFieldType.Column, 3);
            //Draging the fifth field to the data area.
            pivotTable.AddFieldToArea(PivotFieldType.Data, 4);
            //for (int i = 0; i < workbook.Worksheets.Names.Count; i++)
            //{
            //    Console.WriteLine(workbook.Worksheets.Names[i].Text);
            //}
            workbook.Save(Constants.PivotTableDestPath + "Test_165529.xls");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


