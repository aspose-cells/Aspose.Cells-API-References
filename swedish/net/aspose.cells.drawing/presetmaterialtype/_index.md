---
title: "Enum PresetMaterialType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PresetMaterialType enum. Beskriver ytan på en form"
type: docs
url: /sv/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

Beskriver yttre utseende för en form.

```csharp
public enum PresetMaterialType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Clear | `0` | Rensa |
| DarkEdge | `1` | Mörk kant |
| Flat | `2` | Platt |
| LegacyMatte | `3` | Legacy matte |
| LegacyMetal | `4` | Legacy metal |
| LegacyPlastic | `5` | Legacy plastic |
| LegacyWireframe | `6` | Legacy wireframe |
| Matte | `7` | Matt |
| Metal | `8` | Metall |
| Plastic | `9` | Plast |
| Powder | `10` | Pulver |
| SoftEdge | `11` | Mjuk kant |
| SoftMetal | `12` | Mjuk metall |
| TranslucentPowder | `13` | Genomskinligt pulver |
| WarmMatte | `14` | Varm matt |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class PresetMaterialTypeDemo
    {
        public static void PresetMaterialTypeExample()
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

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Få åtkomst till den första serien i diagrammet
            Series series = chart.NSeries[0];

            // Få åtkomst till seriens 3D-format
            Format3D format3D = series.ShapeProperties.Format3D;

            // Ställ in ytmaterialtyp
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Ställ in andra 3D-egenskaper
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Spara arbetsboken
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Skriv ut resultaten
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


