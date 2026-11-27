---
title: "Enum PivotItemPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotItemPositionType-enum. Representerar positionstypen för pivotbasobjektet i basfältet när ShowDataAs-beräkning används."
type: docs
url: /sv/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

Representerar positionstypen för pivotbasobjektet i basfältet när ShowDataAs‑beräkningen används.

```csharp
public enum PivotItemPositionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Previous | `0` | Representerar det föregående pivotobjektet i PivotField. |
| Next | `1` | Representerar nästa pivotobjekt i PivotField. |
| Custom | `2` | Visar värden i olika format baserat på indexet för pivotobjektet i PivotField. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // Ställ in dataformatet för att visa värden som skillnad från föregående objekt
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // Uppdatera och beräkna pivottabellen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


