---
title: PivotTable.SetManualGroupField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Sets manual field group by the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/setmanualgroupfield/
---
## SetManualGroupField(int, double, double, ArrayList, double) {#setmanualgroupfield_2}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(int baseFieldIndex, double startVal, double endVal, 
    ArrayList groupByList, double intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
| startVal | Double | Specifies the starting value for numeric grouping. |
| endVal | Double | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Double | Specifies the interval number group by numeric grouping. |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodSetManualGroupFieldWithInt32DoubleDoubleArrayListDoubDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample numeric data for grouping
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10.5);
            worksheet.Cells["A3"].PutValue(15.2);
            worksheet.Cells["A4"].PutValue(20.7);
            worksheet.Cells["A5"].PutValue(25.1);
            worksheet.Cells["A6"].PutValue(30.9);
            worksheet.Cells["A7"].PutValue(35.4);

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:A7", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            try
            {
                // Prepare parameters for SetManualGroupField
                int baseFieldIndex = 0;
                double startVal = 10.0;
                double endVal = 40.0;
                ArrayList groupByList = new ArrayList() { 10.0 }; // Group by 10s
                double intervalNum = 10.0;

                // Call SetManualGroupField with numeric parameters
                pivotTable.SetManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum);

                // Calculate data to update pivot table
                pivotTable.CalculateData();

                Console.WriteLine("SetManualGroupField executed successfully with numeric parameters");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetManualGroupField: {ex.Message}");
            }

            workbook.Save("PivotTableMethodSetManualGroupFieldDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SetManualGroupField(PivotField, double, double, ArrayList, double) {#setmanualgroupfield}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(PivotField pivotField, double startVal, double endVal, 
    ArrayList groupByList, double intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | Double | Specifies the starting value for numeric grouping. |
| endVal | Double | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Double | Specifies the interval number group by numeric grouping. |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodSetManualGroupFieldWithPivotFieldDoubleDoubleArrayListDoubleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            worksheet.Cells["A3"].Value = new DateTime(2023, 1, 2);
            worksheet.Cells["A4"].Value = new DateTime(2023, 1, 3);
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calculate data to populate the pivot table
            pivotTable.CalculateData();

            try
            {
                // Get the pivot field for grouping
                PivotField pivotField = pivotTable.RowFields[0];

                // Create an ArrayList for group by values
                ArrayList groupByList = new ArrayList();
                groupByList.Add(1.0);
                groupByList.Add(2.0);

                // Call SetManualGroupField with appropriate parameters
                pivotTable.SetManualGroupField(pivotField, 1.0, 3.0, groupByList, 1.0);

                Console.WriteLine("SetManualGroupField method called successfully");

                // Save the workbook to show the effect
                workbook.Save("SetManualGroupFieldDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetManualGroupField: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SetManualGroupField(int, DateTime, DateTime, ArrayList, int) {#setmanualgroupfield_3}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(int baseFieldIndex, DateTime startVal, DateTime endVal, 
    ArrayList groupByList, int intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Int32 | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodSetManualGroupFieldWithInt32DateTimeDateTimeArrayListInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            worksheet.Cells["A3"].Value = new DateTime(2023, 1, 2);
            worksheet.Cells["A4"].Value = new DateTime(2023, 1, 3);
            worksheet.Cells["A5"].Value = new DateTime(2023, 1, 4);
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 1500;
            worksheet.Cells["B4"].Value = 2000;
            worksheet.Cells["B5"].Value = 2500;

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Create an ArrayList for grouping intervals
                ArrayList groupByList = new ArrayList();
                groupByList.Add(PivotGroupByType.Days);

                // Call SetManualGroupField with appropriate parameters
                pivotTable.SetManualGroupField(
                    0, // baseFieldIndex (Date field)
                    new DateTime(2023, 1, 1), // startVal
                    new DateTime(2023, 1, 4), // endVal
                    groupByList, // groupByList
                    1); // intervalNum (group by 1 day)

                Console.WriteLine("SetManualGroupField method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetManualGroupField: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("SetManualGroupFieldDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SetManualGroupField(PivotField, DateTime, DateTime, ArrayList, int) {#setmanualgroupfield_1}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(PivotField pivotField, DateTime startVal, DateTime endVal, 
    ArrayList groupByList, int intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Int32 | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodSetManualGroupFieldWithPivotFieldDateTimeDateTimeArrayListInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Populate sample data with a Date column and an Amount column
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Amount");

            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 15));
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue(new DateTime(2020, 3, 10));
            sheet.Cells["B3"].PutValue(150);
            sheet.Cells["A4"].PutValue(new DateTime(2020, 6, 5));
            sheet.Cells["B4"].PutValue(200);
            sheet.Cells["A5"].PutValue(new DateTime(2020, 9, 20));
            sheet.Cells["B5"].PutValue(180);

            // Create a pivot table based on the data range
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D3", "DemoPivot");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Add the Date field as a row field and Amount as a data field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Get the PivotField that represents the Date column
            PivotField datePivotField = pivotTable.RowFields[0];

            // Prepare parameters for SetManualGroupField
            DateTime startDate = new DateTime(2020, 1, 1);
            DateTime endDate = new DateTime(2020, 12, 31);
            ArrayList groupByList = new ArrayList();
            groupByList.Add("Months");
            groupByList.Add("Quarters");
            int intervalNum = 1; // group interval

            try
            {
                // Call the obsolete SetManualGroupField method
                pivotTable.SetManualGroupField(datePivotField, startDate, endDate, groupByList, intervalNum);

                // Recalculate the pivot table to apply the grouping
                pivotTable.CalculateData();

                Console.WriteLine("SetManualGroupField executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetManualGroupField: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("PivotTable_SetManualGroupField_Demo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


