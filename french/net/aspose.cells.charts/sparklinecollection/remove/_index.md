---
title: "SparklineCollection.Remove"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "SparklineCollection method. Supprime le sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparklinecollection/remove/
---
## SparklineCollection.Remove method

Supprime le sparkline

```csharp
[Obsolete("Use SparklineCollection.RemoveSparkline(Sparkline) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Remove(object o)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| o | Object |  |

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la méthode RemoveSparkline(). Cette méthode sera supprimée 6 mois plus tard à compter de décembre 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionMethodRemoveWithObjectDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Insère des données d'exemple dans la feuille de calcul
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);


            // Définit la CellArea où les sparklines seront ajoutés
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Ajoute un nouveau SparklineGroup à la feuille de calcul
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;

            // Ajoute des sparklines au SparklineGroup
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Définit diverses propriétés pour le SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Définit les couleurs pour les points hauts et bas
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Définit la couleur de la série et l'épaisseur de la ligne
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;


            // Obtenez le premier sparkline à supprimer
            Sparkline sparklineToRemove = sparklineCollection[0];

            // Appelez la méthode Remove avec l'objet sparkline
            sparklineCollection.Remove(sparklineToRemove);

            Console.WriteLine("Sparkline removed successfully");


            Console.WriteLine("after deleted---Sparkline count: " + sparklineCollection.Count);
            // Enregistrez le classeur
            workbook.Save("SparklineRemoveDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


