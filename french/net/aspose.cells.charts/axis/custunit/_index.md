---
title: "Axis.CustUnit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Spécifie une valeur personnalisée pour l'unité d'affichage"
type: docs
url: /fr/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

Spécifie une valeur personnalisée pour l'unité d'affichage.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété Axis.CustomUnit. Cette propriété sera supprimée 12 mois plus tard depuis janvier 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Ajouter un graphique et définir sa plage de données
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Obtenir l'axe des valeurs
            Axis valueAxis = chart.ValueAxis;

            // Afficher la valeur actuelle de CustUnit (propriété obsolète)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // Définir une nouvelle valeur d'unité personnalisée (1,000,000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // Afficher la nouvelle valeur de CustUnit
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // Enregistrer le résultat
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


