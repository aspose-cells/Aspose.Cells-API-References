---
title: "Classe GridExportTableOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridDesktop.Data.GridExportTableOptions classe. Représente toutes les options d'exportation de tableau."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridexporttableoptions/
---
## GridExportTableOptions class

Représente toutes les options d'exportation de tableau.

```csharp
public class GridExportTableOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridExportTableOptions](gridexporttableoptions/)() | constructeur de GridExportTableOptions |

## Propriétés

| Nom | Description |
| --- | --- |
| [CheckMixedValueType](../../aspose.cells.griddesktop.data/gridexporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells définira le type du DataColumn en fonction du type de valeur de la première ligne pour des raisons de performance. True, Aspose.Cells vérifiera si le type de valeur dans la colonne est mixte avant de définir le type du DataColumn. Si les types de valeur sont mixtes, le type du DataColumn sera string. |
| [DataTable](../../aspose.cells.griddesktop.data/gridexporttableoptions/datatable/) { get; set; } | Obtient et définit le DataTable auquel le type de données des colonnes est attribué. |
| [ExportAsHtmlString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportashtmlstring/) { get; set; } | Exporte la valeur de chaîne HTML des cellules vers le DataTable. |
| [ExportAsString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportasstring/) { get; set; } | Exporte la valeur de chaîne des cellules vers le DataTable. |
| [ExportColumnName](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportcolumnname/) { get; set; } | Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. La valeur par défaut est false. |
| [FormatStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/formatstrategy/) { get; set; } | Obtient et définit la stratégie de format lors de l'exportation de la valeur en tant que chaîne. |
| [Indexes](../../aspose.cells.griddesktop.data/gridexporttableoptions/indexes/) { get; set; } | Les index des colonnes/lignes qui doivent être exportés. |
| [IsVertical](../../aspose.cells.griddesktop.data/gridexporttableoptions/isvertical/) { get; set; } | True si une ligne du fichier Workbook représente une ligne dans le DataTable. False si une colonne du fichier Workbook représente une ligne dans le DataTable. |
| [PlotVisibleCells](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecells/) { get; set; } | Exporte uniquement les cellules visibles. |
| [PlotVisibleColumns](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecolumns/) { get; set; } | Exporte uniquement les colonnes visibles. |
| [PlotVisibleRows](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblerows/) { get; set; } | Exporte uniquement les lignes visibles. |
| [RenameStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/renamestrategy/) { get; set; } | Stratégie pour les noms de colonnes en double. |
| [SkipErrorValue](../../aspose.cells.griddesktop.data/gridexporttableoptions/skiperrorvalue/) { get; set; } | Indique s'il faut ignorer les valeurs invalides pour la colonne. Par exemple, si le type de la colonne est décimal, que la valeur dépasse decimal.MaxValue et que cette propriété est true, nous ne lancerons plus d'exception. La valeur par défaut est false. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


