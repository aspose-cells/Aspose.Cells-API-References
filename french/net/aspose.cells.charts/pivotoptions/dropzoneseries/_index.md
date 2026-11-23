---
title: "PivotOptions.DropZoneSeries"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotOptions. Spécifie si un contrôle pour chaque champ de tableau croisé dynamique sur l'axe des colonnes du tableau croisé dynamique source apparaît sur le graphique lorsque dropZonesVisible est défini sur true"
type: docs
url: /fr/net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

Spécifie si un contrôle pour chaque champ de PivotTable sur l'axe des colonnes du PivotTable source apparaît sur le graphique lorsque dropZonesVisible est défini sur true.

```csharp
public bool DropZoneSeries { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneSeriesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et obtenir la première feuille
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(7);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A1:B4", true);
            
            // Obtenir les options de tableau croisé dynamique depuis le graphique
            PivotOptions options = chart.PivotOptions;
            
            // Démontrer la propriété DropZoneSeries
            Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
            options.DropZoneSeries = true;
            Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
            
            // Enregistrez le classeur
            workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


