---
title: "Worksheet.GetFreezedPanes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑metod. Hämtar de frysta rutorna"
type: docs
url: /sv/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

Hämtar frysfönstren.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32& | Radindex. |
| column | Int32& | Kolumnindex. |
| freezedRows | Int32& | Antal synliga rader i översta rutan, högst radindex. |
| freezedColumns | Int32& | Antal synliga kolumner i vänstra rutan, högst kolumnindex. |

### Returvärde

Returnerar om arbetsbladet är fryst

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Frys rutor på cell C5 (rad 4, kolumn 2) med 2 frysta rader och 1 fryst kolumn
            worksheet.FreezePanes(4, 2, 2, 1);

            // Deklarera variabler för att lagra information om de frysta rutorna
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // Anropa GetFreezedPanes‑metoden med ut‑parametrar
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // Visa resultaten
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // Spara arbetsboken
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


