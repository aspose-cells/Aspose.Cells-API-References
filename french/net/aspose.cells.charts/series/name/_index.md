---
title: "Series.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient ou définit le nom de la série de données"
type: docs
url: /fr/net/aspose.cells.charts/series/name/
---
## Series.Name property

Obtient ou définit le nom de la série de données.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des séries au graphique
            chart.NSeries.Add("A2:C2", true);
            
            // Démontrer l'utilisation de la propriété Name
            // 1. Nom de référence d’une cellule
            chart.NSeries[0].Name = "=A1";
            
            // 2. Définir une chaîne comme nom
            chart.NSeries[0].Name = "First Series";
            
            // Enregistrez le classeur
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


