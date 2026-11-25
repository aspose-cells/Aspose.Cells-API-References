---
title: "Enum GradientPresetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.GradientPresetType enum. Rappresenta il tipo di colore predefinito del gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

Rappresenta il tipo di colore predefinito del gradiente.

```csharp
public enum GradientPresetType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Brass | `0` | Colore predefinito Ottone |
| CalmWater | `1` | Colore predefinito Acqua Calma |
| Chrome | `2` | Colore predefinito Cromo |
| ChromeII | `3` | Colore predefinito Cromo II |
| Daybreak | `4` | Colore predefinito Alba |
| Desert | `5` | Colore predefinito Deserto |
| EarlySunset | `6` | Colore predefinito Tramonto Precoce |
| Fire | `7` | Colore predefinito Fuoco |
| Fog | `8` | Colore predefinito Nebbia |
| Gold | `9` | Colore predefinito Oro |
| GoldII | `10` | Colore predefinito Oro II |
| Horizon | `11` | Colore predefinito Orizzonte |
| LateSunset | `12` | Colore predefinito Tramonto Tardivo |
| Mahogany | `13` | Colore predefinito Mogano |
| Moss | `14` | Colore predefinito Muschio |
| Nightfall | `15` | Colore predefinito Tramonto |
| Ocean | `16` | Colore predefinito Oceano |
| Parchment | `17` | Colore predefinito Pergamena |
| Peacock | `18` | Colore predefinito Pavone |
| Rainbow | `19` | Colore predefinito Arcobaleno |
| RainbowII | `20` | Colore predefinito Arcobaleno II |
| Sapphire | `21` | Colore predefinito Zaffiro |
| Silver | `22` | Colore predefinito Argento |
| Wheat | `23` | Colore predefinito Grano |
| Unknown | `24` | Colore predefinito sconosciuto. Solo per il colore predefinito (che non corrisponde a nessun colore predefinito noto) nella cartella di lavoro modello. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
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

            // Accedi all'asse delle categorie del grafico
            Axis categoryAxis = chart.CategoryAxis;

            // Accedi al formato di riempimento dell'area dell'asse delle categorie
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Imposta un colore predefinito a gradiente per il formato di riempimento
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Restituisci il tipo di colore predefinito a gradiente
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Salva la cartella di lavoro
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


