---
title: "Legend.LegendEntries"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Legend. Obtient une collection de tous les objets LegendEntry dans la légende de graphique spécifiée. La définition des entrées de légende du graphique de surface n'est pas prise en charge. Elle renverra donc null si le type de graphique est de type surface."
type: docs
url: /fr/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Obtient une collection de tous les objets LegendEntry dans la légende du graphique spécifié. La définition des entrées de légende du graphique de surface n'est pas prise en charge. Ainsi, elle renverra null si le type de graphique est de type surface.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Accéder aux entrées de légende
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Supprimer la deuxième entrée de légende
            legendEntries[1].IsDeleted = true;
            
            // Enregistrez le classeur
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


