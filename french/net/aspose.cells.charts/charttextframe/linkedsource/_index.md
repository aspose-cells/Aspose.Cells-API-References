---
title: "ChartTextFrame.LinkedSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Obtient et définit une référence à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Obtient et définit une référence à la feuille de calcul.

```csharp
public virtual string LinkedSource { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyLinkedSourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["P1"].PutValue("Chart Title");
            
            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir le titre du graphique et le lier à la cellule P1
            chart.Title.Text = "Linked Title";
            chart.Title.LinkedSource = "='" + worksheet.Name + "'!$P$1";
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier la source liée
            Console.WriteLine("Chart Title Linked Source: " + chart.Title.LinkedSource);
        }
    }
}
```

### Voir aussi

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


