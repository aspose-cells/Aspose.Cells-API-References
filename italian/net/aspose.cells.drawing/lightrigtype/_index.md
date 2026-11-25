---
title: "Enum LightRigType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.LightRigType enum. Rappresenta una luce preimpostata che può essere applicata a una forma"
type: docs
url: /it/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

Rappresenta una luce predefinita a destra che può essere applicata a una forma

```csharp
public enum LightRigType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Balanced | `0` | Bilanciato |
| BrightRoom | `1` | Stanza luminosa |
| Chilly | `2` | Fresco |
| Contrasting | `3` | Contrastante |
| Flat | `4` | Piatto |
| Flood | `5` | Alluvione |
| Freezing | `6` | Gelido |
| Glow | `7` | Bagliore |
| Harsh | `8` | Aspra |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Mattina |
| Soft | `22` | Morbido |
| Sunrise | `23` | Alba |
| Sunset | `24` | Tramonto |
| ThreePoint | `25` | Tre punti |
| TwoPoint | `26` | Due punti |
| None | `27` | Nessuna struttura di illuminazione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Accedi alla prima serie nel grafico
            Series series = chart.NSeries[0];

            // Accedi alle proprietà della forma della serie
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Verifica se la serie ha dati di formato 3D
            if (shapeProperties.HasFormat3D())
            {
                // Accedi alle proprietà del formato 3D
                Format3D format3D = shapeProperties.Format3D;

                // Imposta il tipo di illuminazione della superficie su Bilanciato
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Imposta l'angolo di illuminazione
                format3D.LightingAngle = 45.0;
            }

            // Salva la cartella di lavoro
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Restituisci i risultati
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


