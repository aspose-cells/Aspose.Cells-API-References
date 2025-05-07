---
title: PivotTable.ColumnHeaderCaption
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the Column Header Caption of the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/columnheadercaption/
---
## PivotTable.ColumnHeaderCaption property

Gets the Column Header Caption of the PivotTable.

```csharp
public string ColumnHeaderCaption { get; set; }
```

### Examples

```csharp
// Called: pivotTable.ColumnHeaderCaption = columnField.Name;
[Test]
        public void Property_ColumnHeaderCaption()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA42339_";
            Workbook workbook = new Workbook(filePath + "source.xlsx");
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet tempSheet = workbook.Worksheets[sheetIndex];
            tempSheet.Name = "Sort Asc Top to Bottom By API";
            PivotTableCollection pivotTables = tempSheet.PivotTables;
            // Adding a PivotTable to the worksheet
            int index = pivotTables.Add("=Data!A1:F30", "B3", "SortAscTopToBottom");
            // Accessing the instance of the newly added PivotTable
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); //Employee
            //pivotTable.AddFieldToArea(PivotFieldType.Row, 1); //Quarter
            pivotTable.AddFieldToArea(PivotFieldType.Column, 2); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 5); //Sale

            PivotFieldCollection rowFields = pivotTable.RowFields;
            PivotField rowField = rowFields[0];
            pivotTable.RowHeaderCaption = rowField.Name;
            rowField.IsAutoSubtotals = false;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;//Ascending.
            rowField.AutoSortField = 0; ;//First data field

            PivotFieldCollection columnFields = pivotTable.ColumnFields;
            PivotField columnField = columnFields[0];
            pivotTable.ColumnHeaderCaption = columnField.Name;
            columnField.IsAutoSubtotals = false;
            columnField.IsAutoSort = true;
            columnField.IsAscendSort = true;//Ascending.


            sheetIndex = workbook.Worksheets.Add();
            tempSheet = workbook.Worksheets[sheetIndex];
            tempSheet.Name = "Sort Asc Left to Right By API";

            pivotTables = tempSheet.PivotTables;
            // Adding a PivotTable to the worksheet
            index = pivotTables.Add("=Data!A1:F30", "B3", "SortAscLeftToRight");
            // Accessing the instance of the newly added PivotTable
            pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); //Employee
            //pivotTable.AddFieldToArea(PivotFieldType.Row, 1); //Quarter
            pivotTable.AddFieldToArea(PivotFieldType.Column, 2); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 5); //Sale

            columnFields = pivotTable.ColumnFields;
            columnField = columnFields[0];
            pivotTable.ColumnHeaderCaption = columnField.Name;
            columnField.IsAutoSubtotals = false;
            columnField.IsAutoSort = true;
            columnField.IsAscendSort = true;//Ascending.
            columnField.AutoSortField = 0;//First data field

            rowFields = pivotTable.RowFields;
            rowField = rowFields[0];
            pivotTable.RowHeaderCaption = rowField.Name;
            rowField.IsAutoSubtotals = false;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;//Ascending.

            workbook.Save(CreateFolder(filePath) + "out.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


