---
title: "Legend.IsOverLay"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Legend. Obtient ou définit si la légende est affichée sans chevaucher le graphique"
type: docs
url: /fr/net/aspose.cells.charts/legend/isoverlay/
---
## Legend.IsOverLay property

Obtient ou définit si la légende est affichée sans chevaucher le graphique.

```csharp
public bool IsOverLay { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyIsOverLayDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Définir le chevauchement de la légende
            chart.Legend.IsOverLay = true;
            
            // Enregistrez le classeur
            workbook.Save("LegendOverlayDemo.xlsx");
            
            Console.WriteLine("Chart with overlay legend created successfully.");
        }
    }
}
```

### Voir aussi

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


