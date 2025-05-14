---
title: PivotTable.AutoFormatType
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the auto format type of PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

Gets and sets the auto format type of PivotTable.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### Examples

```csharp
// Called: pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
public void PivotTable_Property_AutoFormatType()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA42587_";

    String file = "Forecast Sets.xlsx";
    int rowCount = 201;
    int colCount = 17;
    String pivotName = "Pivot";

    String[] pageField = {"Forecast Set", "Created By", "Creation Date", "Consume", "Outlier Update Percentage", "Backward Days", "Foreward Days", "Forecast",
            "Forecast Description", "Demand Class", "Customer Name", "Bill Address", "Ship Address", "Disable Date", "Level1"};
    String[] columnField = { "Bucket Type" };
    String[] rowField = { "Organization Code" };
    String[] dataField = { };

    Workbook workbook = new Workbook(filePath + file);
    String sourceData = "'Data'!$A$" + (1) + ":" + CellsHelper.CellIndexToName(rowCount, colCount - 1);

    Worksheet worksheet = workbook.Worksheets.Add(pivotName);
    PivotTableCollection pivotTables = worksheet.PivotTables;
    int index = pivotTables.Add(sourceData, "A10", pivotName);
    PivotTable pivotTable = (PivotTable)pivotTables[index];
    pivotTable.Name = pivotName;

    pivotTable.IsGridDropZones = true;

    for (int i = 0; i < columnField.Length; i++)
    {
        pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields[columnField[i]]);
    }

    for (int i = 0; i < pageField.Length; i++)
    {
        pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields[pageField[i]]);
    }

    for (int i = 0; i < rowField.Length; i++)
    {
        pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[rowField[i]]);
    }

    pivotTable.IsAutoFormat = true;
    pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
    pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
    pivotTable.PageFieldWrapCount = 5;

    for (int i = 0; i < dataField.Length; i++)
    {
        pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[dataField[i]]);
    }

    pivotTable.SaveData = true;
    pivotTable.PreserveFormatting = true;
    workbook.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


