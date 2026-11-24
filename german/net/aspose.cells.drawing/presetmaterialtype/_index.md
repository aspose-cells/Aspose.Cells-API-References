---
title: "Enum PresetMaterialType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.PresetMaterialType enum. Beschreibt das Aussehen der Oberfläche einer Form"
type: docs
url: /de/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

Beschreibt das Oberflächen­aussehen einer Form.

```csharp
public enum PresetMaterialType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Clear | `0` | Löschen |
| DarkEdge | `1` | Dunkle Kante |
| Flat | `2` | Flach |
| LegacyMatte | `3` | Veraltete Matte |
| LegacyMetal | `4` | Veraltetes Metall |
| LegacyPlastic | `5` | Veralteter Kunststoff |
| LegacyWireframe | `6` | Veraltetes Drahtgitter |
| Matte | `7` | Matt |
| Metal | `8` | Metall |
| Plastic | `9` | Kunststoff |
| Powder | `10` | Pulver |
| SoftEdge | `11` | Weiche Kante |
| SoftMetal | `12` | Weiches Metall |
| TranslucentPowder | `13` | Durchscheinendes Pulver |
| WarmMatte | `14` | Warm matt |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Greifen Sie auf die erste Serie im Diagramm zu
            Series series = chart.NSeries[0];

            // Greifen Sie auf das 3D-Format der Serie zu
            Format3D format3D = series.ShapeProperties.Format3D;

            // Legen Sie den Oberflächenmaterialtyp fest
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Legen Sie weitere 3D-Eigenschaften fest
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Speichere die Arbeitsmappe
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Ergebnisse ausgeben
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


