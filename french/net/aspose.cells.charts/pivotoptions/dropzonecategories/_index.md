---
title: "PivotOptions.DropZoneCategories"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotOptions. Spécifie si un contrôle pour chaque champ de tableau croisé dynamique sur l'axe des lignes du tableau croisé dynamique source apparaît sur le graphique lorsque dropZonesVisible est défini sur true"
type: docs
url: /fr/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

Spécifie si un contrôle pour chaque champ de PivotTable sur l'axe des lignes du PivotTable source apparaît sur le graphique lorsque dropZonesVisible est défini sur true.

```csharp
public bool DropZoneCategories { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Ajouter un graphique qui utilise les données du tableau croisé dynamique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Accéder aux options de tableau croisé dynamique depuis le graphique
            PivotOptions options = chart.PivotOptions;
            
            // Démontrer la propriété DropZoneCategories
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // Enregistrez le classeur
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


