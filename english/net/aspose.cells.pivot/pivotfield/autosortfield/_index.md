---
title: PivotField.AutoSortField
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the index of field which is auto sorted. 1 means PivotField itselfothers means the position of the data fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

```csharp
public int AutoSortField { get; set; }
```

### Examples

```csharp
// Called: sortField.AutoSortField = 2;
[Test]
        public void Property_AutoSortField()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA43101_";

            Workbook workbook = new Workbook(filePath + "Unsorted pivot table - input.xlsx");
            Worksheet worksheet = workbook.Worksheets["PivotTable"];

            PivotTable tbl = worksheet.PivotTables[0];


            PivotField sortField = tbl.RowFields[1];
            sortField.IsAutoSort = true;
            sortField.IsAscendSort = false;
            sortField.AutoSortField = 2;

            tbl.RefreshData();
            tbl.CalculateData();

            workbook.Save(CreateFolder(filePath) + "out.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


