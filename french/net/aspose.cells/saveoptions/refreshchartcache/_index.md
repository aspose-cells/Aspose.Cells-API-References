---
title: "SaveOptions.RefreshChartCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Indique s'il faut mettre en cache les dernières données du graphique"
type: docs
url: /fr/net/aspose.cells/saveoptions/refreshchartcache/
---
## SaveOptions.RefreshChartCache property

Indique s'il faut mettre en cache les dernières données du graphique.

```csharp
public bool RefreshChartCache { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyRefreshChartCacheDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec un graphique
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Créer des options d'enregistrement PDF avec RefreshChartCache activé
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.RefreshChartCache = true;

            // Enregistrer le classeur avec l'option de rafraîchissement du cache du graphique
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("Workbook saved with chart cache refreshed.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


