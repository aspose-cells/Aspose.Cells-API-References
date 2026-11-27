---
title: "Enum SparklinePresetStyleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.SparklinePresetStyleType enum. Representerar de förinställda stiltyperna för sparkline"
type: docs
url: /sv/net/aspose.cells.charts/sparklinepresetstyletype/
---
## SparklinePresetStyleType enumeration

Representerar förinställda stiltyper för sparkline.

```csharp
public enum SparklinePresetStyleType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Style1 | `0` | Stil 1 |
| Style2 | `1` | Stil 2 |
| Style3 | `2` | Stil 3 |
| Style4 | `3` | Stil 4 |
| Style5 | `4` | Stil 5 |
| Style6 | `5` | Stil 6 |
| Style7 | `6` | Stil 7 |
| Style8 | `7` | Stil 8 |
| Style9 | `8` | Stil 9 |
| Style10 | `9` | Stil 10 |
| Style11 | `10` | Stil 11 |
| Style12 | `11` | Stil 12 |
| Style13 | `12` | Stil 13 |
| Style14 | `13` | Stil 14 |
| Style15 | `14` | Stil 15 |
| Style16 | `15` | Stil 16 |
| Style17 | `16` | Stil 17 |
| Style18 | `17` | Stil 18 |
| Style19 | `18` | Stil 19 |
| Style20 | `19` | Stil 20 |
| Style21 | `20` | Stil 21 |
| Style22 | `21` | Stil 22 |
| Style23 | `22` | Stil 23 |
| Style24 | `23` | Stil 24 |
| Style25 | `24` | Stil 25 |
| Style26 | `25` | Stil 26 |
| Style27 | `26` | Stil 27 |
| Style28 | `27` | Stil 28 |
| Style29 | `28` | Stil 29 |
| Style30 | `29` | Stil 30 |
| Style31 | `30` | Stil 31 |
| Style32 | `31` | Stil 32 |
| Style33 | `32` | Stil 33 |
| Style34 | `33` | Stil 34 |
| Style35 | `34` | Stil 35 |
| Style36 | `35` | Stil 36 |
| Custom | `36` | Ingen förinställd stil. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklinePresetStyleTypeDemo
    {
        public static void SparklinePresetStyleTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sparkline-diagram
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["D1"].PutValue(4);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["C2"].PutValue(3);
            worksheet.Cells["D2"].PutValue(2);
            worksheet.Cells["E2"].PutValue(1);

            // Definiera CellArea för sparkline-diagrammen
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // Lägg till sparkline-diagram i kalkylbladet
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:E2", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add("A1:E1", 0, 5);
            group.Sparklines.Add("A2:E2", 1, 5);

            // Ange förinställd stiltyp för sparkline-gruppen
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // Spara arbetsboken
            workbook.Save("SparklinePresetStyleTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


