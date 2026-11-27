---
title: "PivotTable.EnableDataValueEditing"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger ett booleskt värde som visar om användaren får redigera cellerna i dataområdet i pivottabellen. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/enabledatavalueediting/
---
## PivotTable.EnableDataValueEditing property

Anger ett booleskt värde som visar om användaren får redigera cellerna i dataområdet i pivottabellen. Standardvärdet är falskt.

```csharp
public bool EnableDataValueEditing { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyEnableDataValueEditingDemo
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
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B5"].PutValue(3000);

            // Lägg till en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella värdet för EnableDataValueEditing
            Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);

            // Aktivera redigering av datavärden
            pivotTable.EnableDataValueEditing = true;

            // Beräkna data för att fylla pivottabellen
            pivotTable.CalculateData();

            // Spara arbetsboken innan redigering
            workbook.Save("PivotTableBeforeEdit.xlsx");

            // Nu kan vi redigera datavärdena direkt i pivottabellen
            // För demonstration kommer vi att ändra en cell i dataområdet
            Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
            if (dataCell != null)
            {
                dataCell.PutValue(2500); // Modify the value
            }

            // Spara arbetsboken efter redigering
            workbook.Save("PivotTableAfterEdit.xlsx");

            // Inaktivera redigering av datavärden
            pivotTable.EnableDataValueEditing = false;
            Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


