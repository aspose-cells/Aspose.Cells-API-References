---
title: "Enum PresetMaterialType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.PresetMaterialType enum. Descrive l'aspetto della superficie di una forma"
type: docs
url: /it/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

Descrive l'aspetto superficiale di una forma.

```csharp
public enum PresetMaterialType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Clear | `0` | Trasparente |
| DarkEdge | `1` | Bordo scuro |
| Flat | `2` | Piatto |
| LegacyMatte | `3` | Legacy opaco |
| LegacyMetal | `4` | Legacy metallo |
| LegacyPlastic | `5` | Legacy plastica |
| LegacyWireframe | `6` | Legacy struttura a reticolo |
| Matte | `7` | Opaco |
| Metal | `8` | Metallo |
| Plastic | `9` | Plastica |
| Powder | `10` | Polvere |
| SoftEdge | `11` | Bordo morbido |
| SoftMetal | `12` | Metallo morbido |
| TranslucentPowder | `13` | Polvere traslucida |
| WarmMatte | `14` | Opaco caldo |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Accedi alla prima serie nel grafico
            Series series = chart.NSeries[0];

            // Accedi al formato 3D della serie
            Format3D format3D = series.ShapeProperties.Format3D;

            // Imposta il tipo di materiale della superficie
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Imposta altre proprietà 3D
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Salva la cartella di lavoro
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Restituisci i risultati
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


