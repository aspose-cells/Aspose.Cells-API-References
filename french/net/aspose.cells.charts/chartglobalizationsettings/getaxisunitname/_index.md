---
title: "ChartGlobalizationSettings.GetAxisUnitName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartGlobalizationSettings. Obtient le nom de l'unité d'axe"
type: docs
url: /fr/net/aspose.cells.charts/chartglobalizationsettings/getaxisunitname/
---
## ChartGlobalizationSettings.GetAxisUnitName method

Obtient le nom de Axis Unit

```csharp
public virtual string GetAxisUnitName(DisplayUnitType type)
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Créer les paramètres de mondialisation et obtenir le nom de l'unité d'axe
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string thousandsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);
            string millionsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Millions);

            // Afficher les résultats
            Console.WriteLine("Thousands unit name: " + thousandsUnit);
            Console.WriteLine("Millions unit name: " + millionsUnit);

            // Enregistrer le classeur
            workbook.Save("AxisUnitNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DisplayUnitType](../../displayunittype/)
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


