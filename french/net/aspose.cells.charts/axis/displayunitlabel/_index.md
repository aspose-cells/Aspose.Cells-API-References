---
title: "Axis.DisplayUnitLabel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente une étiquette d'unité sur un axe dans le graphique spécifié. Les étiquettes d'unité sont utiles pour tracer de grandes valeurs, par exemple en millions ou en milliards"
type: docs
url: /fr/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Représente une étiquette d'unité sur un axe dans le graphique spécifié. Les étiquettes d'unité sont utiles pour tracer de grandes valeurs - par exemple, en millions ou en milliards.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A1:A4", true);
            
            // Configurer l'unité d'affichage et l'étiquette
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Afficher le texte de l'étiquette d'unité d'affichage
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Enregistrez le classeur
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


