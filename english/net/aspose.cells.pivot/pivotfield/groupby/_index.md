---
title: PivotField.GroupBy
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Automatically group the field with internal
type: docs
url: /net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_6}

Automatically group the field with internal

```csharp
public void GroupBy(double interval, bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| interval | Double | The internal of group. Automatic value will be assigned if it's zero, |
| newField | Boolean | Indicates whether adding a new field to the pivottable. |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Create a workbook from source Excel file
            Workbook workbook = new Workbook("example.xlsx");
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access the first pivot table
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Add field to column area
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Group the field by 1 (interval) with automatic range
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_5}

Automatically group the field with internal

```csharp
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| groups | PivotGroupByType[] | Group types |
| interval | Double | The internal of group. Automatic value will be assigned if it's zero, |
| newField | Boolean | Indicates whether adding a new field to the pivottable. |

### See Also

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_4}

Group the file by the date group types.

```csharp
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start datetime |
| end | DateTime | The end of datetime |
| groups | PivotGroupByType[] | Group types |
| interval | Double | The interval |
| firstAsNewField | Boolean | Indicates whether adding a new field to the pivottable. Only for the first group item. |

### Return Value

False means this field could not be grouped by date time.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with dates for pivot table
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Get the pivot field
            PivotField pivotField = pivotTable.RowFields[0];

            // Prepare parameters for GroupBy method
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // Call GroupBy method with date parameters
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Refresh pivot table
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_2}

Group the file by the date group types.

```csharp
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isAutoStart | Boolean | Indicates whether to auto detect the start date time value. |
| start | DateTime | The start datetime |
| isAutoEnd | Boolean | Indicates whether to auto detect the end date time value. |
| end | DateTime | The end of datetime |
| groups | PivotGroupByType[] | Group types |
| interval | Double | The interval |
| firstAsNewField | Boolean | Indicates whether adding a new field to the pivottable. Only for the first group item. |

### Return Value

False means this field could not be grouped by date time.

### See Also

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_3}

Group the file by number.

```csharp
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | Double | The start value |
| end | Double | The end of value |
| interval | Double | The interval |
| newField | Boolean | Indicates whether adding a new field to the pivottable |

### Return Value

False means this field could not be grouped by date time.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add row field and group it
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Save the workbook
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_1}

Group the file by number.

```csharp
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isAutoStart | Boolean | Indicates whether to auto detect the start value. |
| start | Double | The start value |
| isAutoEnd | Boolean | Indicates whether to auto detect the end value. |
| end | Double | The end of value |
| interval | Double | The interval |
| newField | Boolean | Indicates whether adding a new field to the pivottable |

### Return Value

False means this field could not be grouped by date time.

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Custom group the field.

```csharp
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | The custom group items. |
| newField | Boolean | Indicates whether adding a new field to the pivottable |

### Return Value

False means this field could not be grouped by date time.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Get the pivot field
            PivotField pivotField = pivotTable.RowFields[0];

            // Create custom group items
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Call GroupBy method with custom group items
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Refresh pivot table
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### See Also

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


