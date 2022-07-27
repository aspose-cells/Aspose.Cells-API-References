---
title: GridTableItemStyle
second_title: Référence de l'API Aspose.Cells pour .NET
description: Hérité de System.Web.UI.WebControls.TableItemStyle. Encapsule les styles dun WebCell.
type: docs
weight: 780
url: /fr/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Hérité de System.Web.UI.WebControls.TableItemStyle. Encapsule les styles d'un WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle)() | Constructeur par défaut. |

## Propriétés

| Nom | La description |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes) { get; set; } | Attributs de l'image d'arrière-plan. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl) { get; set; } | URL de l'image de fond. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle) { get; set; } | Spécifie le style de la bordure inférieure de la cellule. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom) { get; set; } | Obtient ou définit le format personnalisé, une chaîne nulle ou vide signifie qu'il n'y a pas de format personnalisé. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel) { get; set; } | Obtient ou définit le niveau d'indentation. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked) { get; set; } | Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non lorsque sa feuille de calcul est protégée. Lorsque sa feuille de calcul est protégée et que IsLocked vaut true, la cellule ne peut pas être modifiée. Lorsque sa feuille de calcul est protégée et que IsLocked est faux, la cellule peut être modifiée. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle) { get; set; } | Spécifie le style de la bordure gauche de la cellule. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype) { get; set; } | Obtient ou définit le format d'affichage des nombres et des dates. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle) { get; set; } | Spécifie le style de la bordure droite de la cellule. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle) { get; set; } | Obtient ou définit l'attribut Rotation. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle) { get; set; } | Spécifie le style de la bordure supérieure de la cellule. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender#addattributestorender_1)(HtmlTextWriter, WebControl) | Usage interne uniquement. Méthode d'implémentation Ne pas appeler cette méthode directement. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom)(Style) | Copies d'un autre objet de style. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode)() | Sert de fonction de hachage pour un type particulier, adapté à une utilisation dans les algorithmes de hachage et les structures de données comme une table de hachage. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith)(Style) | Fusionne avec un autre objet de style. |

### Exemples

```csharp
[C#]
...
using System.Web.UI.WebControls;
...
...
WebWorksheets sheets = GridWeb1.WebWorksheets;
sheets.Clear();
WebWorksheet sheet = sheets[sheets.Add("demo1")];

WebCell cell = sheet.Cells[0,0];
cell.StringValue = "Demo Text";

Aspose.Cells.GridWeb.TableItemStyle style = cell.GetStyle();
style.Font.Size = new FontUnit("72pt");
style.Wrap = false;

style.BackColor = Color.Gray;
style.BorderStyle = BorderStyle.Solid;
style.BorderWidth = new Unit(1, UnitType.Pixel);
style.BorderColor = Color.Silver;

style.RightBorderStyle.BorderColor = Color.Black;
style.RightBorderStyle.BorderStyle = BorderStyle.Solid;
style.RightBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
style.BottomBorderStyle.BorderColor = Color.Black;
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid;
style.BottomBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
cell.SetStyle(style);

[Visual Basic]
...
Imports System.Web.UI.WebControls
...
...
Dim sheets As WebWorksheets =  GridWeb1.WebWorksheets
sheets.Clear()
Dim sheet As WebWorksheet =  sheets(sheets.Add(__0__))

Dim cell As WebCell =  sheet.Cells(0,0)
cell.StringValue = "Demo Text"

Dim style As Aspose.Cells.GridWeb.TableItemStyle = cell.GetStyle()
style.Font.Size = New FontUnit("72pt")
style.Wrap = False

style.BackColor = Color.Gray
style.BorderStyle = BorderStyle.Solid
style.BorderWidth = New Unit(1, UnitType.Pixel)
style.BorderColor = Color.Silver

style.RightBorderStyle.BorderColor = Color.Black
style.RightBorderStyle.BorderStyle = BorderStyle.Solid
style.RightBorderStyle.BorderWidth = New Unit(1, UnitType.Pixel)
style.BottomBorderStyle.BorderColor = Color.Black
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid
style.BottomBorderStyle.BorderWidth = New Unit(1, UnitType.Pixel)
cell.SetStyle(style)
```

### Voir également

* espace de noms [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* Assemblée [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
