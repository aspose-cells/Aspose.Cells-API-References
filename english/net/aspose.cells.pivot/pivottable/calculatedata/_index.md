---
title: PivotTable.CalculateData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Calculates data of pivottable to cells
type: docs
url: /net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata}

Calculates data of pivottable to cells.

```csharp
public void CalculateData()
```

### Remarks

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Create pivot table - fixed by ensuring correct parameters
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add fields to pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Apply date filter
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Calculate pivot data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Save the workbook
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata_1}

Calculates pivot table with options.

```csharp
public void CalculateData(PivotTableCalculateOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableCalculateOption | The options for calculating the pivot table |

### Remarks

If PivotTableCalculateOption.RefreshData is true, this method will refresh pivot cache from data source,then calculate all pivot tables based same pivot cache.

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configure pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Set calculation options
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculate with options
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


