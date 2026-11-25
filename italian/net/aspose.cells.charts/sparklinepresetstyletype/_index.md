---
title: "Enum SparklinePresetStyleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.SparklinePresetStyleType enum. Rappresenta i tipi di stile predefiniti per sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinepresetstyletype/
---
## SparklinePresetStyleType enumeration

Rappresenta i tipi di stile predefiniti per lo sparkline.

```csharp
public enum SparklinePresetStyleType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Style1 | `0` | Stile 1 |
| Style2 | `1` | Stile 2 |
| Style3 | `2` | Stile 3 |
| Style4 | `3` | Stile 4 |
| Style5 | `4` | Stile 5 |
| Style6 | `5` | Stile 6 |
| Style7 | `6` | Stile 7 |
| Style8 | `7` | Stile 8 |
| Style9 | `8` | Stile 9 |
| Style10 | `9` | Stile 10 |
| Style11 | `10` | Stile 11 |
| Style12 | `11` | Stile 12 |
| Style13 | `12` | Stile 13 |
| Style14 | `13` | Stile 14 |
| Style15 | `14` | Stile 15 |
| Style16 | `15` | Stile 16 |
| Style17 | `16` | Stile 17 |
| Style18 | `17` | Stile 18 |
| Style19 | `18` | Stile 19 |
| Style20 | `19` | Stile 20 |
| Style21 | `20` | Stile 21 |
| Style22 | `21` | Stile 22 |
| Style23 | `22` | Stile 23 |
| Style24 | `23` | Stile 24 |
| Style25 | `24` | Stile 25 |
| Style26 | `25` | Stile 26 |
| Style27 | `26` | Stile 27 |
| Style28 | `27` | Stile 28 |
| Style29 | `28` | Stile 29 |
| Style30 | `29` | Stile 30 |
| Style31 | `30` | Stile 31 |
| Style32 | `31` | Stile 32 |
| Style33 | `32` | Stile 33 |
| Style34 | `33` | Stile 34 |
| Style35 | `34` | Stile 35 |
| Style36 | `35` | Stile 36 |
| Custom | `36` | Nessuno stile predefinito. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per le sparklines
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

            // Definisci il CellArea per le sparklines
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // Aggiungi sparklines al foglio di lavoro
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:E2", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add("A1:E1", 0, 5);
            group.Sparklines.Add("A2:E2", 1, 5);

            // Imposta il tipo di stile predefinito del gruppo di sparklines
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // Salva la cartella di lavoro
            workbook.Save("SparklinePresetStyleTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


