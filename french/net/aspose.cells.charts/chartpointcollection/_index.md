---
title: "Classe ChartPointCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.ChartPointCollection. Représente une collection contenant tous les points d’une série"
type: docs
url: /fr/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Représente une collection qui contient tous les points d'une série.

```csharp
public class ChartPointCollection : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Obtient le nombre de points du graphique. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Obtient l'élément [`ChartPoint`](../chartpoint/) à l'index spécifié dans la série. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Supprime tous les paramètres des points du graphique. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Renvoie un énumérateur pour l’ensemble `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Supprime le point à l'index de la série. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Obtention de la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];

            // Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);

            // Afficher les étiquettes de données
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Accéder à la ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Itérer à travers les points de la collection
            for (int i = 0; i < points.Count; i++)
            {
                // Obtenir le point de données
                ChartPoint point = points[i];
                
                // Définir l'explosion du secteur
                point.Explosion = 15;
                
                // Définir la couleur de bordure
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Enregistrement du fichier Excel
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


