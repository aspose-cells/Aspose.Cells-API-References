---
title: "Classe GridHtmlSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions. Représente les options pour enregistrer un fichier html"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Représente les options pour enregistrer le fichier HTML.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | Crée des options pour enregistrer un fichier html. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | Crée des options pour enregistrer un fichier htm. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | Le répertoire où les fichiers joints seront enregistrés. Uniquement pour l'enregistrement dans un flux html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Spécifiez le préfixe d'URL des fichiers joints tels que les images dans le fichier html. Uniquement pour l'enregistrement dans un flux html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | Le dossier de fichiers en cache est utilisé pour stocker de grandes données. (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l'enregistrement du fichier. (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | Spécifiez le nom de police par défaut pour l'exportation html, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | Si non défini, utilisez Encoding.UTF8 comme type d'encodage par défaut. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indique si l'exportation du classeur complet vers un fichier html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | Obtient ou définit la zone de cellules exportée de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille de calcul active actuelle sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | Indiquant si l'exportation des quadrillages est activée. La valeur par défaut est false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | Indique si les en-têtes sont exportés lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indiquant si l'exportation du contenu de la feuille de calcul masquée est activée. La valeur par défaut est true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | Spécifie si les images sont enregistrées au format Base64 vers HTML, MHTML ou EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | Indique si seule la zone d'impression est exportée vers le fichier html. La valeur par défaut est false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | Indique si l'exportation d'un seul onglet est activée lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | Indique s’il faut exporter les commentaires lors de l’enregistrement du fichier en HTML, la valeur par défaut est false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | Indique s’il faut utiliser un lien avec chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | Le titre de la page HTML. Seulement lors de l’enregistrement dans un flux HTML. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | Analyse les balises html dans la cellule, comme <br>, en tant que valeur de cellule, ou en tant que balise html, la valeur par défaut est true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | Indique si les données du cache du graphique sont rafraîchies (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | Obtient le format de fichier d'enregistrement. (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | Indique si le tri des noms définis est effectué avant d'enregistrer le fichier. (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | Indique si la validation des cellules fusionnées est effectuée avant d'enregistrer le fichier. (Hérité de [`GridSaveOptions`](../gridsaveoptions/).) |

### Voir aussi

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


