---
title: DataBar
second_title: Référence de l'API Aspose.Cells pour .NET
description: Décrire la règle de mise en forme conditionnelle de DataBar. Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules.
type: docs
weight: 1240
url: /fr/net/aspose.cells/databar/
---
## DataBar class

Décrire la règle de mise en forme conditionnelle de DataBar. Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules.

```csharp
public class DataBar
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | Obtient la couleur de l'axe pour les cellules avec mise en forme conditionnelle sous forme de barres de données. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | Obtient ou définit la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | Obtient un objet qui spécifie la bordure d'une barre de données. |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | Obtient ou définit la manière dont une barre de données est remplie de couleur. |
| [Color](../../aspose.cells/databar/color) { get; set; } | Obtenir ou définir la couleur de cette DataBar. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | Obtient ou définit la direction d'affichage de la barre de données. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | Obtenir ou définir l'objet de valeur maximale de cette DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | Représente la longueur maximale de la barre de données. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | Obtenir ou définir l'objet de valeur minimale de cette DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | Représente la longueur minimale de la barre de données. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | Obtient l'objet NegativeBarFormat associé à une règle de mise en forme conditionnelle de la barre de données. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | Obtenir ou définir l'indicateur indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée. La valeur par défaut est true. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | Rendre la barre de données dans la cellule en tableau d'octets d'image. |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Ajoute une mise en forme conditionnelle vide
int index = sheet.ConditionalFormattings.Add();

FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

// Définit la plage de format conditionnel.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

//Ajoute une condition.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

//Obtenir la barre de données
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

//Définir les propriétés de la barre de données
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;

dataBar.MinCfvo.Value = 30;

dataBar.ShowValue = false;

dataBar.BarBorder.Type = DataBarBorderType.Solid;

dataBar.BarBorder.Color = Color.Plum;

 dataBar.BarFillType = DataBarFillType.Solid;
  
 dataBar.AxisColor = Color.Red;
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.Color = Color.White;
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
 
// Placer les valeurs des cellules
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

//Enregistrement du fichier Excel
workbook.Save("book1.xlsx");

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Ajoute une mise en forme conditionnelle vide
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'Définit la plage de format conditionnel.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'Ajoute un état.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'Obtenir la barre de données
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'Définir les propriétés de la barre de données
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile

dataBar.MinCfvo.Value = 30

dataBar.ShowValue = False

dataBar.BarBorder.Type = DataBarBorderType.Solid

dataBar.BarBorder.Color = Color.Plum

 dataBar.BarFillType = DataBarFillType.Solid
  
 dataBar.AxisColor = Color.Red
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.Color = Color.White
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow

'Mettre les valeurs des cellules
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'Enregistrement du fichier Excel
workbook.Save("book1.xlsx")

```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
