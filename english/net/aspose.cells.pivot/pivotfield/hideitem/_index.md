---
title: PivotField.HideItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specific PivotItem in a data field is hidden
type: docs
url: /net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Sets whether the specific PivotItem in a data field is hidden.

```csharp
public void HideItem(int index, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the pivotItem in the pivotField. |
| isHidden | Boolean | whether the specific PivotItem is hidden |

### Examples

```csharp
// Called: pf.HideItem(i, pf.Items[i] != "PO-23-05");
public void PivotField_Method_HideItem()
{
    Workbook wb = new Workbook(Constants.openPivottablePath + "wec3.xls");
    Workbook wb1 = new Workbook(Constants.openPivottablePath + "basis+PO.xls");
    Worksheet wsin = wb.Worksheets[0];
    PivotTable pt = wsin.PivotTables["Draaitabel2"];
    PivotField pf = pt.RowFields[0];
    for (int i = 0; i < pf.ItemCount; i++)
    {
        pf.HideItem(i, pf.Items[i] != "PO-23-05");
    }

    pt.CalculateData();
    pt.CalculateRange();

    Worksheet wsout = wb1.Worksheets["Ambulante begeleiding"];
    Aspose.Cells.Range rin = wsin.Cells.CreateRange(pt.TableRange1.StartRow + 1, pt.TableRange1.StartColumn, pt.TableRange1.EndRow - pt.TableRange1.StartRow - 1, pt.TableRange1.EndColumn - pt.TableRange1.StartColumn + 1);
    Aspose.Cells.Range rout = wsout.Cells.CreateRange(2, 0, pt.TableRange1.EndRow - pt.TableRange1.StartRow - 1, pt.TableRange1.EndColumn - pt.TableRange1.StartColumn + 1);
    rout.CopyData(rin);
    rout.CopyStyle(rin);


    wb.Save(Constants.savePivottablePath + "example.xls");
    wb1.Save(Constants.savePivottablePath + "example.xls");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Sets whether the specific PivotItem in a data field is hidden.

```csharp
public void HideItem(string itemValue, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | String | the value of the pivotItem in the pivotField. |
| isHidden | Boolean | whether the specific PivotItem is hidden |

### Examples

```csharp
namespace AsposeCellsExamples.PivotFieldMethodHideItemWithStringBooleanDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodHideItemWithStringBooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Get the pivot field
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Call the HideItem method with parameters (String, Boolean)
                pivotField.HideItem("Apple", true);

                Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
                Console.WriteLine("Apple items are now hidden in the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HideItem method: {ex.Message}");
            }

            // Save the result
            workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


