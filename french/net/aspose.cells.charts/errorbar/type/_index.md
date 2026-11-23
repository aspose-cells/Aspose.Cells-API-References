---
title: "ErrorBar.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ErrorBar. Représente le type de quantité de la barre d'erreur"
type: docs
url: /fr/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Représente le type de quantité de la barre d'erreur.

```csharp
public ErrorBarType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // Créer un graphique
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // Ajouter des données de série
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // Définir le type et les valeurs de la barre d'erreur personnalisée
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // Enregistrez le classeur
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


