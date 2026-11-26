---
title: "Enumeración SparklinePresetStyleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.SparklinePresetStyleType enum. Representa los tipos de estilo predefinidos para sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinepresetstyletype/
---
## SparklinePresetStyleType enumeration

Representa los tipos de estilo predefinidos para la sparkline.

```csharp
public enum SparklinePresetStyleType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Style1 | `0` | Estilo 1 |
| Style2 | `1` | Estilo 2 |
| Style3 | `2` | Estilo 3 |
| Style4 | `3` | Estilo 4 |
| Style5 | `4` | Estilo 5 |
| Style6 | `5` | Estilo 6 |
| Style7 | `6` | Estilo 7 |
| Style8 | `7` | Estilo 8 |
| Style9 | `8` | Estilo 9 |
| Style10 | `9` | Estilo 10 |
| Style11 | `10` | Estilo 11 |
| Style12 | `11` | Estilo 12 |
| Style13 | `12` | Estilo 13 |
| Style14 | `13` | Estilo 14 |
| Style15 | `14` | Estilo 15 |
| Style16 | `15` | Estilo 16 |
| Style17 | `16` | Estilo 17 |
| Style18 | `17` | Estilo 18 |
| Style19 | `18` | Estilo 19 |
| Style20 | `19` | Estilo 20 |
| Style21 | `20` | Estilo 21 |
| Style22 | `21` | Estilo 22 |
| Style23 | `22` | Estilo 23 |
| Style24 | `23` | Estilo 24 |
| Style25 | `24` | Estilo 25 |
| Style26 | `25` | Estilo 26 |
| Style27 | `26` | Estilo 27 |
| Style28 | `27` | Estilo 28 |
| Style29 | `28` | Estilo 29 |
| Style30 | `29` | Estilo 30 |
| Style31 | `30` | Estilo 31 |
| Style32 | `31` | Estilo 32 |
| Style33 | `32` | Estilo 33 |
| Style34 | `33` | Estilo 34 |
| Style35 | `34` | Estilo 35 |
| Style36 | `35` | Estilo 36 |
| Custom | `36` | Sin estilo predefinido. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para sparklines
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

            // Definir el CellArea para los sparklines
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // Agregar sparklines a la hoja de cálculo
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:E2", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add("A1:E1", 0, 5);
            group.Sparklines.Add("A2:E2", 1, 5);

            // Establecer el tipo de estilo predefinido del grupo de sparklines
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // Guarda el libro de trabajo
            workbook.Save("SparklinePresetStyleTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


