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

    public class PivotTableMethodSetManualGroupFieldWithPivotFieldDoubleDoubleArrayLisDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample numeric data for grouping
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(5.5);
            worksheet.Cells["A3"].PutValue(12.3);
            worksheet.Cells["A4"].PutValue(18.7);
            worksheet.Cells["A5"].PutValue(24.9);
            worksheet.Cells["A6"].PutValue(32.1);
            worksheet.Cells["A7"].PutValue(39.6);

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:A7", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add row field and get the pivot field
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Prepare parameters for SetManualGroupField
                double startVal = 5.0;
                double endVal = 40.0;
                ArrayList groupByList = new ArrayList() { 10.0 }; // Group by 10s
                double intervalNum = 10.0;

                // Call SetManualGroupField with PivotField parameter
                pivotTable.SetManualGroupField(pivotField, startVal, endVal, groupByList, intervalNum);

                // Calculate data to update pivot table
                pivotTable.CalculateData();

                Console.WriteLine("SetManualGroupField executed successfully with PivotField parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetManualGroupField: {ex.Message}");
            }

            workbook.Save("PivotTableMethodSetManualGroupFieldWithPivotFieldDemo.xlsx");
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

    public class PivotTableMethodSetManualGroupFieldWithInt32DateTimeDateTimeArrayListDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with dates for grouping
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2200);

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Prepare parameters for SetManualGroupField
                int baseFieldIndex = 0; // Index of Date field
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 4, 30);
                ArrayList groupByList = new ArrayList { 1, 2 }; // Group by months and quarters
                int intervalNum = 1; // Interval number

                // Call SetManualGroupField with specified parameters
                pivotTable.SetManualGroupField(baseFieldIndex, startDate, endDate, groupByList, intervalNum);

                Console.WriteLine("SetManualGroupField executed successfully with parameters (Int32, DateTime, DateTime, ArrayList, Int32)");

                // Calculate data to show the effect
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetManualGroupField method: {ex.Message}");
            }

            // Save the result
            workbook.Save("PivotTableMethodSetManualGroupFieldWithInt32DateTimeDateTimeArrayListDemo.xlsx");
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
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodSetManualGroupFieldWithPivotFieldDateTimeDateTimeArraDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2008, 1, 13, 0, 32, 14));
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue(new DateTime(2010, 5, 15, 12, 15, 30));
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue(new DateTime(2012, 9, 20, 8, 45, 0));
            sheet.Cells["B4"].PutValue(300);
            sheet.Cells["A5"].PutValue(new DateTime(2014, 7, 5, 1, 0, 0));
            sheet.Cells["B5"].PutValue(400);

            // Create pivot table
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Add fields
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Configure grouping
            ArrayList groupByList = new ArrayList();
            groupByList.Add(PivotGroupByType.Years);
            groupByList.Add(PivotGroupByType.Months);

            DateTime startDate = new DateTime(2008, 1, 1);
            DateTime endDate = new DateTime(2014, 12, 31);
            
            // Apply manual grouping
            pivotTable.SetManualGroupField(pivotTable.BaseFields[0], startDate, endDate, groupByList, 1);

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


