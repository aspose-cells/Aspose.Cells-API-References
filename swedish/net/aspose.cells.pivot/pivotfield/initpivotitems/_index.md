---
title: "PivotField.InitPivotItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Initiera pivotelementen för pivottfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/initpivotitems/
---
## PivotField.InitPivotItems method

Initiera pivotelementen för pivottfältet

```csharp
[Obsolete("Please simply remove calling this method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void InitPivotItems()
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Vänligen ta helt enkelt bort anropet av denna metod. Metoden kommer att tas bort 6 månader senare från och med oktober 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodInitPivotItemsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Initiera pivotelement
                pivotField.InitPivotItems();

                // Visa pivotelementen
                Console.WriteLine("Pivot Items after initialization:");
                foreach (PivotItem item in pivotField.PivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Spara arbetsboken
                workbook.Save("PivotFieldInitPivotItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitPivotItems method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


