---
title: "Enum ShiftType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ShiftType enum. Representerar skiftalternativen när ett cellområde tas bort"
type: docs
url: /sv/net/aspose.cells/shifttype/
---
## ShiftType enumeration

Representerar förskjutningsalternativen när ett cellområde tas bort.

```csharp
public enum ShiftType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Down | `0` | Skifta celler nedåt. |
| Left | `1` | Skifta celler åt vänster. |
| None | `2` | Skifta inte celler. |
| Right | `3` | Skifta celler åt höger. |
| Up | `4` | Skifta celler uppåt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Infoga en ny rad på index 1 och skifta befintliga rader nedåt
            worksheet.Cells.InsertRows(1, 1, true);

            // Ange ett värde i den nyinfogade raden
            worksheet.Cells["A1"].PutValue("New Item");

            // Ta bort ett cellområde och flytta cellerna uppåt
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // Skriv ut de återstående värdena i den första kolumnen
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // Spara arbetsboken
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


