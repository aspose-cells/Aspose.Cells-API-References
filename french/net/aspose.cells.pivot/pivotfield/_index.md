---
title: PivotField
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente un champ dans un rapport de tableau croisé dynamique.
type: docs
weight: 4530
url: /fr/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Représente un champ dans un rapport de tableau croisé dynamique.

```csharp
public class PivotField
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | Représente le nombre d'éléments supérieurs ou inférieurs qui sont automatiquement affichés dans le champ de tableau croisé dynamique spécifié. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | Représente l'index de champ d'affichage automatique. -1 signifie PivotField lui-même. Ce devrait être l'index des champs de données. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | Représente l'index de champ de tri automatique. -1 signifie PivotField lui-même, les autres signifient la position des champs de données. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | Représente le champ de base pour un calcul personnalisé. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | Représente l'index PivotField dans la base PivotFields. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | Représente l'élément dans le champ de base pour un calcul personnalisé. Valable uniquement pour les champs de données. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | Représente l'élément dans le champ de base pour un calcul personnalisé. Valable uniquement pour les champs de données. Étant donné que PivotItemPosition.Custom est uniquement en lecture, si vous devez définir PivotItemPosition.Custom, veuillez définir l'attribut PivotField.BaseItemIndex. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | Représente l'élément de page actuel affiché pour le champ de page (valable uniquement pour les champs de page). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | Représente comment afficher les valeurs contenues dans un champ de données. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | Représente le nom d'affichage PivotField. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | Indique si le champ spécifié peut être déplacé vers la position de la colonne. La valeur par défaut est true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | Indique si le champ spécifié peut être déplacé vers la position des données. La valeur par défaut est true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | Indique si le champ spécifié peut être déplacé vers la position masquée. La valeur par défaut est true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | Indique si le champ spécifié peut être déplacé vers la position de la page. La valeur par défaut est true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | Indique si le champ spécifié peut être déplacé vers la position de ligne. La valeur par défaut est true. |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | Représente la fonction utilisée pour résumer le champ de données du tableau croisé dynamique. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | Indique s'il faut insérer une ligne vierge après chaque élément. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | Indique si le champ de tableau croisé dynamique spécifié s'affiche automatiquement en ordre croissant. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | Indique si le champ de tableau croisé dynamique spécifié est trié automatiquement par ordre croissant. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | Indique si le champ de tableau croisé dynamique spécifié est automatiquement affiché, uniquement valable pour Excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | Indique si le champ de tableau croisé dynamique spécifié est trié automatiquement. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | Indique si le champ spécifié affiche des sous-totaux automatiques. La valeur par défaut est true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | Indique si le champ de tableau croisé dynamique spécifié est un champ calculé. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | indique si le champ peut inclure de nouveaux éléments dans le filtre manuel La valeur par défaut est false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | indique si le champ peut insérer des sauts de page entre les items insérer un saut de page après chaque item La valeur par défaut est false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | indique si le champ peut avoir plusieurs items sélectionnés dans la page field La valeur par défaut est false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | indique si le champ peut répéter des éléments labels La valeur par défaut est false. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | Obtient le nombre d'éléments de base de ce champ pivot. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | Obtenir tous les éléments de base ; |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | Représente le nom du PivotField. |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | Représente le format d'affichage intégré des nombres et des dates. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | Représente le format d'affichage personnalisé des nombres et des dates. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | Obtenir les éléments de base d'origine ; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | Obtient les éléments pivots du champ pivot |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | Représente l'index PivotField dans PivotFields. |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | Obtient la plage de groupe du champ pivot |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | Indique si tous les éléments du rapport de tableau croisé dynamique sont affichés, même s'ils ne contiennent pas de données récapitulatives. affiche les éléments sans données La valeur par défaut est false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | Indique si les étiquettes d'affichage du champ suivant dans la même colonne sur la vue Tableau croisé dynamique |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | Indique si la disposition de ce champ sous forme de plan sur la vue Tableau croisé dynamique |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | lorsque ShowInOutlineForm est vrai, alors affiche les sous-totaux en haut de la liste des éléments au lieu d'en bas |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | Ajouter un élément calculé au champ pivot. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | Obtenir la chaîne de formule du champ calculé spécifié . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | Obtient le filtre pivot du champ pivot par type |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | Obtient les filtres de pivot du champ pivot |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | Obtient si le champ spécifié affiche ces sous-totaux. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | Définit si les PivotItems d'un champ pivot sont des détails masqués. C'est-à-dire réduire/développer ce champ. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | Définit si le PivotItem spécifique dans un champ de données est masqué. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | Définit si le PivotItem spécifique dans un champ de données est masqué. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | Définit si le PivotItem spécifique dans un champ pivot est un détail caché. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | Init les éléments pivot du champ pivot |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | Indique si le PivotItem spécifique est masqué. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | Indique si le PivotItem spécifique est un détail caché. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | Définit si le champ spécifié affiche les sous-totaux. |

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

//Modifier les attributs de PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

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

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Voir également

* espace de noms [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
