---
title: Area
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente un format de zone.
type: docs
weight: 1760
url: /fr/net/aspose.cells.drawing/area/
---
## Area class

Encapsule l'objet qui représente un format de zone.

```csharp
public class Area
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor) { get; set; } | Obtient ou définit l'arrière-planColor de la[`Area`](../area) . |
| [FillFormat](../../aspose.cells.drawing/area/fillformat) { get; } | Représente un objet qui contient les propriétés de formatage de remplissage pour le graphique ou la forme spécifié. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor) { get; set; } | Obtient ou définit le premier planColor . |
| [Formatting](../../aspose.cells.drawing/area/formatting) { get; set; } | Représente la mise en forme de la zone. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative) { get; set; } | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif, la couleur de premier plan et la couleur d'arrière-plan seront échangées. |
| [Transparency](../../aspose.cells.drawing/area/transparency) { get; set; } | Renvoie ou définit le degré de transparence de la zone sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair). |

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
//Ajout d'une nouvelle feuille de calcul à l'objet Workbook
int sheetIndex = workbook.Worksheets.Add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Ajout d'un exemple de valeur à la cellule "A1"
worksheet.Cells["A1"].PutValue(50);
//Ajout d'un exemple de valeur à la cellule "A2"
worksheet.Cells["A2"].PutValue(100);
//Ajout d'un exemple de valeur à la cellule "A3"
worksheet.Cells["A3"].PutValue(150);
//Ajout d'un exemple de valeur à la cellule "B1"
worksheet.Cells["B1"].PutValue(60);
//Ajout d'un exemple de valeur à la cellule "B2"
worksheet.Cells["B2"].PutValue(32);
//Ajout d'un exemple de valeur à la cellule "B3"
worksheet.Cells["B3"].PutValue(50);
//Ajout d'un graphique à la feuille de calcul
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.Charts[chartIndex];
//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
chart.NSeries.Add("A1:B3", true);
//Définition de la couleur de premier plan de la zone de tracé
chart.PlotArea.Area.ForegroundColor = Color.Blue;
//Définition de la couleur de premier plan de la zone du graphique
chart.ChartArea.Area.ForegroundColor = Color.Yellow;
//Définition de la couleur de premier plan de la 1ère zone NSeries
chart.NSeries[0].Area.ForegroundColor = Color.Red;
//Définition de la couleur de premier plan de la zone du 1er point NSeries
chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
//Enregistrement du fichier Excel
workbook.Save("book1.xls");

[Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Ajout d'une nouvelle feuille de calcul à l'objet Workbook
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Obtenir la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Ajouter un graphique à la feuille de calcul
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accéder à l'instance du graphique nouvellement ajouté
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)
'Définition de la couleur de premier plan de la zone de tracé
chart.PlotArea.Area.ForegroundColor = Color.Blue
'Définition de la couleur de premier plan de la zone de graphique
chart.ChartArea.Area.ForegroundColor = Color.Yellow
'Réglage de la couleur de premier plan de la 1ère zone NSeries
chart.NSeries(0).Area.ForegroundColor = Color.Red
'Définition de la couleur de premier plan de la zone du 1er point NSeries
chart.NSeries(0).Points(0).Area.ForegroundColor = Color.Cyan
'Enregistrement du fichier Excel
workbook.Save("book1.xls")
```

### Voir également

* espace de noms [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
