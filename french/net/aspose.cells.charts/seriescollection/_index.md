---
title: SeriesCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule une collection deSeries./series objets.
type: docs
weight: 830
url: /fr/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Encapsule une collection de[`Series`](../series) objets.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | Obtient ou définit la plage des valeurs de l'axe des catégories. Il peut s'agir d'une plage de cellules (telle que "d1:e10"), ou d'une séquence de valeurs (telle que "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | Représente si la couleur des points est variée. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | Obtient le[`Series`](../series) élément à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | Obtient ou définit la plage des valeurs Axis de deuxième catégorie. Il peut s'agir d'une plage de cellules (telle que "d1:e10"), ou d'une séquence de valeurs (telle que "{2,6,8,10}"). Effets uniquement lorsque certaines ASeries tracent sur le deuxième axe. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | Ajoute le[`SeriesCollection`](../seriescollection) collection à un graphique. |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | Ajoute le[`SeriesCollection`](../seriescollection) collection à un graphique. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | Ajoute le[`SeriesCollection`](../seriescollection) collection à un graphique. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | Modifie directement les ordres des deux séries. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | Efface la collection (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | Obtient le[`Series`](../series) élément par commande. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | Supprimer à une série à l'index spécifique. (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | Définit le nom de toutes les séries du graphique. |

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
//Ajout d'une nouvelle feuille de calcul à l'objet Excel
int sheetIndex = workbook.Worksheets.Add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Ajout d'un exemple de valeur à la cellule "A1"
worksheet.Cells["A1"].PutValue(50);
//Ajout d'un exemple de valeur à la cellule "A2"
worksheet.Cells["A2"].PutValue(100);
//Ajout d'un exemple de valeur à la cellule "A3"
worksheet.Cells["A3"].PutValue(150);
//Ajout d'un exemple de valeur à la cellule "A4"
worksheet.Cells["A4"].PutValue(200);
//Ajout d'un exemple de valeur à la cellule "B1"
worksheet.Cells["B1"].PutValue(60);
//Ajout d'un exemple de valeur à la cellule "B2"
worksheet.Cells["B2"].PutValue(32);
//Ajout d'un exemple de valeur à la cellule "B3"
worksheet.Cells["B3"].PutValue(50);
//Ajout d'un exemple de valeur à la cellule "B4"
worksheet.Cells["B4"].PutValue(40);
//Ajout d'un exemple de valeur à la cellule "C1" en tant que données de catégorie
worksheet.Cells["C1"].PutValue("Q1");
//Ajout d'un exemple de valeur à la cellule "C2" en tant que données de catégorie
worksheet.Cells["C2"].PutValue("Q2");
//Ajout d'un exemple de valeur à la cellule "C3" en tant que données de catégorie
worksheet.Cells["C3"].PutValue("Y1");
//Ajout d'un exemple de valeur à la cellule "C4" en tant que données de catégorie
worksheet.Cells["C4"].PutValue("Y2");
//Ajout d'un graphique à la feuille de calcul
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.Charts[chartIndex];
//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B4"
chart.NSeries.Add("A1:B4", true);
//Définition de la source de données pour les données de catégorie de NSeries
chart.NSeries.CategoryData = "C1:C4";
//Enregistrement du fichier Excel
workbook.Save("book1.xls");

[Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Ajout d'une nouvelle feuille de calcul à l'objet Excel
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Obtenir la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Ajouter un graphique à la feuille de calcul
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accéder à l'instance du graphique nouvellement ajouté
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Définition de la source de données pour les données de catégorie de NSeries
chart.NSeries.CategoryData = "C1:C4"
'Enregistrement du fichier Excel
workbook.Save("book1.xls")
```

### Voir également

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* espace de noms [Aspose.Cells.Charts](../../aspose.cells.charts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
