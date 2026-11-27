---
title: "Enum PasteType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PasteType enum. Representerar specialklistringstypen"
type: docs
url: /sv/net/aspose.cells/pastetype/
---
## PasteType enumeration

Representerar specialklistringstypen.

```csharp
public enum PasteType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| All | `0` | Kopierar all data i området. |
| Default | `1` | Det fungerar som "All"-beteende i MS Excel. |
| AllExceptBorders | `2` | Kopierar all data i området utan området. |
| DefaultExceptBorders | `3` | Det fungerar som "All except borders"-beteende i MS Excel. |
| ColumnWidths | `4` | Kopierar endast bredden på området. |
| RowHeights | `5` | Kopierar endast höjderna i intervallet. |
| Comments | `6` | Kopierar endast kommentarer i intervallet. |
| Formats | `7` | Kopierar endast format i intervallet. |
| Formulas | `8` | Kopierar endast formler i intervallet. |
| FormulasAndNumberFormats | `9` | Kopierar endast formler och talformat i intervallet. |
| Validation | `10` | Kopierar endast valideringar i intervallet. |
| Values | `11` | Kopierar endast värden i intervallet. |
| ValuesAndFormats | `12` | Kopierar endast värden och format i intervallet. |
| ValuesAndNumberFormats | `13` | Kopierar endast värden och talformat i intervallet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Definiera källintervallet
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Definiera destinationsintervallet
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // Skapa PasteOptions och ange PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Kopiera källintervallet till destinationsintervallet med de angivna PasteOptions
            destinationRange.Copy(sourceRange, pasteOptions);

            // Spara arbetsboken
            workbook.Save("PasteTypeExample.xlsx");

            // Skriv ut resultaten
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


