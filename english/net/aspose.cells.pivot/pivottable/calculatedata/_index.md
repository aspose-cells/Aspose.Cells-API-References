---
title: PivotTable.CalculateData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Calculates pivottables data to cells
type: docs
url: /net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata}

Calculates pivottable's data to cells.

```csharp
public void CalculateData()
```

### Remarks

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### Examples

```csharp
// Called: pivot.CalculateData();
public void PivotTable_Method_CalculateData()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    //Add PivotFilter
    PivotField field = pivot.ColumnFields[0];
    field.FilterByDate(PivotFilterType.November, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));

    pivot.RefreshData();
    pivot.CalculateData();
    Assert.AreEqual("11/16/2021", book.Worksheets[0].Cells["B17"].StringValue);
    book.Save(Constants.destPath + "November.xlsx");
    book.Save(Constants.destPath + "November.pdf");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata_1}

Calculating pivot tables with options

```csharp
public void CalculateData(PivotTableCalculateOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableCalculateOption |  |

### Examples

```csharp
// Called: pivotTable.CalculateData(calculateOption);
public static void PivotTable_Method_CalculateData()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a PivotTable to the worksheet
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Add fields to the PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Set the ReserveMissingPivotItemType option
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculate the PivotTable with the specified options
            pivotTable.CalculateData(calculateOption);

            // Refresh the PivotTable
            pivotTable.RefreshData();

            // Save the workbook
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
```

### See Also

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


