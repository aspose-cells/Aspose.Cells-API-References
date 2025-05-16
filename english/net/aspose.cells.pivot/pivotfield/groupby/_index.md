---
title: PivotField.GroupBy
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Automatically group the field with internal
type: docs
url: /net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_3}

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
// Called: pt.BaseFields[2].GroupBy(1, true);
public void PivotField_Method_GroupBy()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
            
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    pt.AddFieldToArea(PivotFieldType.Column, 2);
    pt.BaseFields[2].GroupBy(1, true);
    Assert.AreEqual(4, pt.BaseFields.Count);
    Assert.AreEqual("Apr", workbook.Worksheets[0].Cells["G15"].StringValue);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_2}

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
namespace AsposeCellsExamples.PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
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

## GroupBy(double, double, double, bool) {#groupby_1}

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
// Called: pivotTable.RowFields[0].GroupBy(1, 6, 2, false);
public void PivotField_Method_GroupBy()
{
    var wb = new Workbook(Constants.openPivottablePath + "a.xlsx");
    Aspose.Cells.Pivot.PivotTable pivotTable = wb.Worksheets[0].PivotTables[0];
    ArrayList list = new ArrayList();
    list.Add(PivotGroupByType.RangeOfValues);
    //pivotTable.SetManualGroupField(0, 1, 6, list, 2);
    // pivotTable.SetUngroup(0);
    pivotTable.RowFields[0].GroupBy(1, 6, 2, false);
   // pivotTable.BaseFields[0]
    wb.Save(Constants.savePivottablePath + "TestGroup.xlsx");

}
```

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
namespace AsposeCellsExamples.PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
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


