---
title: ListObject
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente un objet de liste dans une feuille de calcul. Lobjet ListObject est membre de la collection ListObjects. La collection ListObjects contient tous les objets de liste dune feuille de calcul.
type: docs
weight: 5820
url: /fr/net/aspose.cells.tables/listobject/
---
## ListObject class

Représente un objet de liste dans une feuille de calcul. L'objet ListObject est membre de la collection ListObjects. La collection ListObjects contient tous les objets de liste d'une feuille de calcul.

```csharp
public class ListObject
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Obtient et définit la description alternative. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Obtient et définit le texte alternatif. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Obtient le filtre automatique. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Obtient et définit le commentaire de la table. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | Obtient la plage de données du ListObject. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Obtient le type de source de données de la table. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Obtient et définit le nom d'affichage. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Obtient la colonne de fin de la plage. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Obtient la dernière ligne de la plage. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | Obtient les ListColumns du ListObject. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Obtient le QueryTable lié. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Obtient et définit si ce ListObject affiche la ligne d'en-tête. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Indique si le format de bande de colonne est appliqué. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Indique si la première colonne du tableau doit avoir le style appliqué. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Indique si la dernière colonne du tableau doit avoir le style appliqué. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Indique si la mise en forme des bandes de lignes est appliquée. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Obtient et définit si ce ListObject affiche la ligne totale. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Obtient la colonne de début de la plage. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Obtient la ligne de début de la plage. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Obtient et définit le nom du style de tableau. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Obtient et le style de tableau intégré. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Obtient un[`XmlMap`](./xmlmap)utilisé pour cette liste. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Appliquer le style de tableau à la plage. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Convertir le tableau en plage. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Convertir le tableau en plage. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Filtrer le tableau. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Mettez la valeur dans la cellule. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Redimensionner la plage de l'objet liste. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Met à jour le nom de toutes les colonnes de la liste à partir de la feuille de calcul. |

### Exemples

```csharp

[C#]


Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
cells[0,i].PutValue(CellsHelper.ColumnIndexToName(i));
 }
for (int row = 1; row  <10; row++)
{
 for (int column = 0; column  <5; column++)
{
cells[row, column].PutValue(row * column);
 }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
 cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
 For column As Int32 = 0 To 4
  cells(row, column).PutValue(row * column)
Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTotals = True
table.ListColumns(4).TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum
workbook.Save("Book1.xlsx")
```

### Voir également

* espace de noms [Aspose.Cells.Tables](../../aspose.cells.tables)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
