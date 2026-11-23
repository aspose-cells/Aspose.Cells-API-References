---
title: "Classe RowFilterSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridWeb.Data.RowFilterSettings class. Description résumée pour RowFilter"
type: docs
url: /fr/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

Description résumée pour RowFilter.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | La chaîne de critères du filtre. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Active le filtrage automatique. La HeaderRow affichera des boutons déroulants pour permettre à l'utilisateur de sélectionner la valeur de la colonne à filtrer. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | Le numéro de ligne de fin de la plage de filtrage. Si cette valeur est définie à -1, le dernier numéro de ligne de la feuille est utilisé. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | Le numéro de ligne d'en-tête qui affichera les boutons déroulants du filtre. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | Le numéro de ligne de début de la plage de filtrage. |

## Méthodes

| Nom | Description |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Construit la chaîne de critères à partir des paramètres du filtre automatique. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Efface tous les paramètres de filtrage et affiche toutes les lignes. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Spécifie un filtre personnalisé. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Filtre les lignes en utilisant la chaîne de critères. |

### Remarques

NOTE : Cette classe est maintenant obsolète. Cette classe sera supprimée après 6 mois à compter d'août 2014. Vous pouvez utiliser GridWorksheet AddAutoFilter/FilterString pour les paramètres de filtrage automatique /filtrage personnalisé. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


