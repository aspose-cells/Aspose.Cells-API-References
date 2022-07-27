---
title: TxtSaveOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les options denregistrement pour csv/délimité par des tabulations/autre format de texte.
type: docs
weight: 6130
url: /fr/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

Représente les options d'enregistrement pour csv/délimité par des tabulations/autre format de texte.

```csharp
public class TxtSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions#constructor)() | Crée des options d'enregistrement de fichier texte. |
| [TxtSaveOptions](txtsaveoptions#constructor_1)(SaveFormat) | Crée des options d'enregistrement de fichier texte. |

## Propriétés

| Nom | La description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Videz le classeur après avoir enregistré le fichier. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Si vrai et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier. |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding) { get; set; } | Obtient et définit l'encodage par défaut. |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets) { get; set; } | Indique si toutes les feuilles sont exportées vers le fichier texte. Si la valeur est fausse, exportez uniquement la feuille active, tout comme MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea) { get; set; } | La plage de cellules à exporter. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix) { get; set; } | Indique si le guillemet simple doit être exporté dans le cadre de la valeur d'une cellule lorsque[`QuotePrefix`](../style/quoteprefix) est vrai pour cela. La valeur par défaut est false. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy) { get; set; } | Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule sous forme de chaîne. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow) { get; set; } | Indique si les séparateurs doivent être sortis pour une ligne vide. La valeur par défaut est false, donc par défaut le contenu de la ligne vide sera vide. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider) { get; set; } | Le fournisseur de données pour fournir des données de cellules pour enregistrer le classeur en mode léger. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indique si fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype) { get; set; } | Obtient ou définit comment citer les valeurs dans le fichier texte exporté. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indique si l'actualisation des données du cache du graphique |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Obtient le format du fichier de sauvegarde. |
| [Separator](../../aspose.cells/txtsaveoptions/separator) { get; set; } | Obtient et définit le délimiteur char du fichier texte. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring) { get; set; } | Obtient et définit une valeur de chaîne comme séparateur. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indique si le tri des noms définis externes avant d'enregistrer le fichier. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indique si le tri des noms définis avant d'enregistrer le fichier. |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn) { get; set; } | Indique si les premières lignes et colonnes vides doivent être coupées comme ce que fait MS Excel. La valeur par défaut est true. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells) { get; set; } | Indique si les cellules vides de fin d'une ligne doivent être supprimées. La valeur par défaut est false. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indique si la mise à jour du paramètre Smart Art. La valeur par défaut est false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indique si valider les cellules fusionnées avant d'enregistrer le fichier. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Obtient ou définit un rappel d'avertissement. |

### Voir également

* class [SaveOptions](../saveoptions)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
