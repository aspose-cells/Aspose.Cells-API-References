---
title: "Classe TrendlineCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.TrendlineCollection. Représente une collection de tous les objets Trendline pour la série de données spécifiée"
type: docs
url: /fr/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

Représente une collection de tous les objets [`Trendline`](../trendline/) pour la série de données spécifiée.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item/) { get; } | Obtient un objet [`Trendline`](../trendline/) par son index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add)(TrendlineType) | Ajoute un objet [`Trendline`](../trendline/) à cette collection avec le type spécifié. |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add_1)(TrendlineType, string) | Ajoute un objet [`Trendline`](../trendline/) à cette collection avec le type et le nom spécifiés. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Trendline) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Trendline, IComparer&lt;Trendline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Trendline, IComparer&lt;Trendline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Trendline) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Trendline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Trendline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Trendline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Trendline&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Trendline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Trendline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Trendline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineCollectionDemo
    {
        public static void TrendlineCollectionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            
            // Ajout d'une nouvelle feuille de calcul à l'objet Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Ajoute NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B4"
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);
            
            // Ajout d'une ligne de tendance à la première série
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Définition des propriétés de la ligne de tendance
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Enregistrement du fichier Excel
            workbook.Save("TrendlineCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Trendline](../trendline/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


