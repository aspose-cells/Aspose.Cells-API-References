---
title: GridHtmlSaveOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les options denregistrement du fichier html.
type: docs
weight: 250
url: /fr/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Représente les options d'enregistrement du fichier html.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | Crée des options pour enregistrer le fichier html. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | Crée des options pour enregistrer le fichier htm. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | Le répertoire dans lequel les fichiers joints seront enregistrés. Uniquement pour l'enregistrement dans le flux html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | Spécifiez le préfixe d'URL des fichiers joints tels que l'image dans le fichier html. Uniquement pour l'enregistrement dans le flux html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | Videz le classeur après avoir enregistré le fichier. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | Si vrai et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | Spécifiez le nom de la police par défaut pour l'exportation html, la police par défaut sera utilisée lorsque la police de style n'existe pas, Si cette propriété est nulle, Aspose.Cells utilisera une police universelle qui a la même famille que la police d'origine, la valeur par défaut est null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | Si non défini, utilisez Encoding.UTF8 comme type d'encodage par défaut. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indique si l'intégralité du classeur est exportée vers un fichier html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | Obtient ou définit la CellArea d'exportation de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille de calcul active actuelle sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | Indique si le quadrillage est exporté. La valeur par défaut est false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | Indique si les en-têtes sont exportés lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | Indique si le contenu masqué de la feuille de calcul est exporté. La valeur par défaut est true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | Spécifie si les images sont enregistrées au format Base64 au format HTML, MHTML ou EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | Indique s'il s'agit d'exporter uniquement la zone d'impression vers un fichier html. La valeur par défaut est false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | Indique s'il faut exporter l'onglet unique lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | Indique si l'exportation des commentaires lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | Indique si le lien de chemin d'accès complet est utilisé dans sheet00x.htm,filelist.xml et tabstrip.htm. La valeur par défaut est false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | Indique si fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | Le titre de la page html. Uniquement pour l'enregistrement dans le flux html. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | Analyser la balise html dans la cellule, comme , en tant que valeur de cellule ou en tant que balise html, la valeur par défaut est true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false.if you want to get plus belle présentation, veuillez définir la valeur sur true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | Indique si l'actualisation des données du cache du graphique |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | Obtient le format du fichier de sauvegarde. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | Indique si le tri des noms définis avant d'enregistrer le fichier. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | Indique si valider les cellules fusionnées avant d'enregistrer le fichier. |

### Voir également

* class [GridSaveOptions](../gridsaveoptions)
* espace de noms [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* Assemblée [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
