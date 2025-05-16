---
title: PivotTable.RemoveField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Removes a field from specific field area
type: docs
url: /net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Removes a field from specific field area

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| fieldName | String | The name in the base fields. |

### Examples

```csharp
// Called: pt.RemoveField(PivotFieldType.Data, "c");
public void PivotTable_Method_RemoveField()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets["Sheet3"].PivotTables[0];
    pt.RemoveField(PivotFieldType.Data, "c");
    pt.CalculateData();
    Assert.AreEqual("0", workbook.Worksheets["Sheet3"].Cells["C4"].StringValue);
    pt = workbook.Worksheets["Sheet1"].PivotTables[0];
    pt.RemoveField(PivotFieldType.Data, "c");
    pt.CalculateData();
    Assert.AreEqual("0", workbook.Worksheets["Sheet1"].Cells["H11"].StringValue);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Removes a field from specific field area

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| baseFieldIndex | Int32 | The field index in the base fields. |

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Remove the row field (index 0) from the pivot table
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Remove field from specific field area

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the fields area type. |
| pivotField | PivotField | the field in the base fields. |

### Examples

```csharp
// Called: wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Column, wb.Worksheets[0].PivotTables[0].ColumnFields[0]);
public void PivotTable_Method_RemoveField()
{
    var wb = new Workbook(Constants.openPivottablePath + "TestFile.xlsx");
    wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Data, wb.Worksheets[0].PivotTables[0].DataFields[0]);
    wb.Save(Constants.savePivottablePath + "example.xlsx");


    wb = new Workbook(Constants.openPivottablePath + "example.xlsx");
    wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Column, wb.Worksheets[0].PivotTables[0].ColumnFields[0]);
    wb.Save(Constants.savePivottablePath + "example.xlsx");
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


