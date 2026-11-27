---
title: "PivotField.HideItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Ställer in om den specifika PivotItem i ett datafält är dold"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Anger om det specifika PivotItem i ett datafält är dolt.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(int index, bool isHidden)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | indexet för pivotItem i pivotField. |
| isHidden | Boolean | om det specifika PivotItem är dolt |

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotField.PivotItems[int].IsHidden. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med ett exempel på pivottabell
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Exempeldatat för pivottabell
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("PO-23-05");
            sheet.Cells["A3"].PutValue("PO-23-06");
            sheet.Cells["A4"].PutValue("PO-23-05");
            sheet.Cells["A5"].PutValue("PO-23-07");
            
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(1500);
            sheet.Cells["B5"].PutValue(3000);

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Dölj objekt som inte är "PO-23-05"
            for (int i = 0; i < pivotField.ItemCount; i++)
            {
                pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
            }
            
            // Beräkna pivottabell
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldHideItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Anger om det specifika PivotItem i ett datafält är dolt.

```csharp
[Obsolete("Use PivotField.PivotItems[string].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(string itemValue, bool isHidden)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| itemValue | String | Namnet på pivotItem i pivotField. |
| isHidden | Boolean | Om den specifika PivotItem är dold |

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotField.PivotItems[string].IsHidden. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodHideItemWithStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
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

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Anropa HideItem-metoden med parametrarna (String, Boolean)
                pivotField.HideItem("Apple", true);

                Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
                Console.WriteLine("Apple items are now hidden in the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HideItem method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


