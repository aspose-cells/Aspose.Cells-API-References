---
title: Slicer
second_title: Référence de l'API Aspose.Cells pour .NET
description: description sommaire de la vue Slicer
type: docs
weight: 5630
url: /fr/net/aspose.cells.slicers/slicer/
---
## Slicer class

description sommaire de la vue Slicer

```csharp
public class Slicer
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | Renvoie ou définit la chaîne de texte descriptive (alternative) de l'objet Slicer. |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | Renvoie ou définit la légende du segment spécifié. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | Renvoie ou définit si l'en-tête qui affiche la légende du segment est visible la valeur par défaut est true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | Renvoie ou définit la largeur, en points, de chaque colonne du segment. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | Obtient ou définit la largeur en unité de pixels pour chaque colonne du segment. |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | Renvoie ou définit la hauteur du segment spécifié, en points. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | Renvoie ou définit la hauteur du segment spécifié, en pixels. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | Indique si la forme du slicer est verrouillée. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | Indique si l'objet slicer est imprimable. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | Renvoie ou définit le décalage horizontal de la forme du segment par rapport à sa colonne de gauche, en pixels. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | Indique si le format d'image est verrouillé. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | Indique si le segment spécifié peut être déplacé ou redimensionné à l'aide de l'interface utilisateur. |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | Renvoie ou définit le nom du slicer spécifié |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | Renvoie ou définit le nombre de colonnes dans le segment spécifié. |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | Renvoie l'objet Worksheet qui représente la feuille contenant le segment. Lecture seule. |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | Représente la manière dont l'objet dessin est attaché aux cellules situées en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | Renvoie ou définit la hauteur, en points, de chaque ligne dans le segment spécifié. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | Renvoie ou définit la hauteur, en pixels, de chaque ligne dans le segment spécifié. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | Renvoie l'objet SlicerCache associé au slicer. Lecture seule. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | Spécifiez le type de style de trancheuse intégré le type par défaut est SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | Spécifie le titre de l'objet Slicer actuel. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | Renvoie ou définit le décalage vertical de la forme du segment par rapport à sa ligne supérieure, en pixels. |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | Renvoie ou définit la largeur du segment spécifié, en points. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | Renvoie ou définit la largeur du segment spécifié, en pixels. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | Ajoute une connexion au tableau croisé dynamique. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | Actualisation du slicer. Pendant ce temps, actualisation et calcul des tableaux croisés dynamiques relatifs. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | Supprime la connexion au tableau croisé dynamique. |

### Exemples

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
SlicerCacheItem item = items[0];
item.Selected = false;
//faites vos affaires
book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10
pivot.RefreshData()
pivot.CalculateData()

Dim slicers As SlicerCollection = sheet.Slicers
Dim slicerIndex As Int32 = slicers.Add(pivot, "E12", "fruit")
Dim slicer As Slicer = slicers(slicerIndex)
slicer.StyleType = SlicerStyleType.SlicerStyleLight2

Dim items As SlicerCacheItemCollection = slicer.SlicerCache.SlicerCacheItems
Dim item As SlicerCacheItem = items(0)
item.Selected = False

book.Save("out_vb.xlsx")
```

### Voir également

* espace de noms [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
