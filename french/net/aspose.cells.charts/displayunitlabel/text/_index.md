---
title: "DisplayUnitLabel.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DisplayUnitLabel. Obtient ou définit le texte du libellé d'unité d'affichage"
type: docs
url: /fr/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Obtient ou définit le texte de l'étiquette d'unité d'affichage.

```csharp
public override string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A1:A4", true);
            
            // Configurer le libellé d'unité d'affichage
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Accéder et modifier le texte du libellé d'unité d'affichage
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // Modifier le texte
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // Enregistrez le classeur
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


