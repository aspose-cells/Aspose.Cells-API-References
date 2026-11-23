---
title: "Enum DisplayUnitType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Charts.DisplayUnitType. Représente le type d'unité d'affichage des axes des graphiques"
type: docs
url: /fr/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

Représente le type d'unité d'affichage de l'axe du graphique.

```csharp
public enum DisplayUnitType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | L'unité d'affichage est Aucune. |
| Hundreds | `1` | Spécifie que les valeurs du graphique doivent être divisées par 100. |
| Thousands | `2` | Spécifie que les valeurs du graphique doivent être divisées par 1 000. |
| TenThousands | `3` | Spécifie que les valeurs du graphique doivent être divisées par 10 000. |
| HundredThousands | `4` | Spécifie que les valeurs du graphique doivent être divisées par 100 000. |
| Millions | `5` | Spécifie que les valeurs du graphique doivent être divisées par 1 000 000. |
| TenMillions | `6` | Spécifie que les valeurs du graphique doivent être divisées par 10 000 000. |
| HundredMillions | `7` | Spécifie que les valeurs du graphique doivent être divisées par 100 000 000. |
| Billions | `8` | Spécifie que les valeurs du graphique doivent être divisées par 1 000 000 000. |
| Trillions | `9` | Spécifie que les valeurs du graphique doivent être divisées par 1 000 000 000 000. |
| Percentage | `10` | Les valeurs du graphique doivent être divisées par 0,01. |
| Cust | `11` | spécifie une valeur personnalisée pour l'unité d'affichage. |
| Custom | `12` | spécifie une valeur personnalisée pour l'unité d'affichage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une nouvelle feuille de calcul au classeur
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajoutez NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Définir l'unité d'affichage de l'axe des valeurs sur Millions
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Facultativement, afficher l'étiquette de l'unité d'affichage
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Enregistrez le classeur
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


