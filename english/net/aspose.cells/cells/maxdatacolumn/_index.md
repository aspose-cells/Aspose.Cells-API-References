---
title: Cells.MaxDataColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum column index of cell which contains data
type: docs
url: /net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Maximum column index of cell which contains data.

```csharp
public int MaxDataColumn { get; }
```

### Remarks

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### Examples

```csharp
// Called: List<Vehicle> vehicles = ExportList<Vehicle>(workbook.Worksheets[0].Cells, 0, 0, cells.MaxDataRow, cells.MaxDataColumn);
public void Property_MaxDataColumn()
        {
            string dir = Constants.sourcePath + @"SmartMarker\";
            Workbook workbook = new Workbook(dir + "repaccs1.csv");
            Cells cells = workbook.Worksheets[0].Cells;
            List<Accident> accidents = ExportList<Accident>(workbook.Worksheets[0].Cells, 0, 0, cells.MaxDataRow, cells.MaxDataColumn);

             workbook = new Workbook(dir + "repvehs1.csv");
             cells = workbook.Worksheets[0].Cells;
            List<Vehicle> vehicles = ExportList<Vehicle>(workbook.Worksheets[0].Cells, 0, 0, cells.MaxDataRow, cells.MaxDataColumn);

             workbook = new Workbook(dir + "repcas1.csv");
             cells = workbook.Worksheets[0].Cells;
            List<Casualty> casualties = ExportList<Casualty>(workbook.Worksheets[0].Cells, 0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            Merge(vehicles, casualties);
            Merge(accidents, vehicles);
            Workbook template = new Workbook(dir + "CELLSNET54674.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(template);
            designer.LineByLine = false;
            designer.SetDataSource("Accidents", accidents);
            designer.Process();
            template.CalculateFormula();
            AssertHelper.AreEqual("Wet/Damp", template.Worksheets[0].Cells["A38"].StringValue,"");
            template.Save(Constants.destPath + "CELLSNET54674.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


