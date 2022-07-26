---
title: PdfSaveOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les options denregistrement du fichier pdf.
type: docs
weight: 4500
url: /fr/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Représente les options d'enregistrement du fichier pdf.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | Crée les options d'enregistrement du fichier pdf. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | Si AllColumnsInOnePagePerSheet est true , tout le contenu de la colonne d'une feuille sortira sur une seule page de résultat. La largeur de la taille du papier de pagesetup sera ignorée et les autres paramètres de pagesetup prendront toujours effet. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | Obtient et définit le[`PdfSignetEntrée`](../../aspose.cells.rendering/pdfbookmarkentry) objet. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | Indique s'il faut calculer les formules avant d'enregistrer le fichier pdf. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, Ils peuvent apparaître sous forme de bloc dans pdf,image. Définissez ceci sur true pour essayer d'utiliser la police par défaut du classeur pour afficher ces caractères en premier. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Videz le classeur après avoir enregistré le fichier. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | Le classeur convertit en pdf selon PdfCompliance dans cette propriété. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Si vrai et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | Obtient et définit l'heure de génération du document pdf. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | Obtient ou définit une valeur déterminant la manière[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) sont exportés vers un fichier PDF. La valeur par défaut est Aucune. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | Obtient ou définit la langue d'édition par défaut. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, Ils peuvent apparaître sous forme de bloc dans pdf,image. Définissez la police par défaut telle que MingLiu ou MS Gothic pour afficher ces caractères. Si cette propriété est non défini, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | Indique si la barre de titre de la fenêtre doit afficher le titre du document. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True pour intégrer des polices True Type. Affecte uniquement les caractères ASCII 32-127. Les polices pour les codes de caractères supérieurs à 127 sont toujours incorporées. Les polices sont toujours incorporées pour la norme PDF/A-1a, PDF/A-1b. La valeur par défaut est true. |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | Paramètre pour le rendu du métafichier Emf. |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | Indique s'il faut exporter la structure du document. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | Obtient ou définit l'encodage de la police intégrée dans le pdf. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | Obtient ou définit le type de quadrillage. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut être une erreur de forme, d'image, de rendu de graphique, etc. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | Indique s'il faut uniquement remplacer la police de caractère lorsque la police de cellule n'est pas compatible avec celle-ci. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indique si fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | Si OnePagePerSheet est true , tout le contenu d'une feuille sortira sur une seule page de résultat. Le format de papier de pagesetup ne sera pas valide et les autres paramètres de pagesetup prendront toujours effet. |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | Obtient et définit le type d'optimisation pdf. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | Indique s'il faut imprimer une page vierge lorsqu'il n'y a rien à imprimer. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | Obtient ou définit l'index de base 0 de la première page à enregistrer. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | Contrôler/Indiquer la progression du processus d'enregistrement de la page. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | Indiquez l'algorithme de compression |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | Indique quelles pages ne seront pas imprimées. |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | Obtient et définit le producteur du document pdf généré. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indique si l'actualisation des données du cache du graphique |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Obtient le format du fichier de sauvegarde. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | Définissez ces options, lorsque la sécurité est nécessaire dans le résultat xls2pdf. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indique si le tri des noms définis externes avant d'enregistrer le fichier. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indique si le tri des noms définis avant d'enregistrer le fichier. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | Obtient ou définit l'affichage du type de texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indique si la mise à jour du paramètre Smart Art. La valeur par défaut est false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indique si valider les cellules fusionnées avant d'enregistrer le fichier. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Obtient ou définit un rappel d'avertissement. |

## Méthodes

| Nom | La description |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | Définit le PPI souhaité (pixels par pouce) des images de rééchantillonnage et la qualité jpeg. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié, et les images supérieures au PPI spécifié (pixels par pouce) seront rééchantillonnées. |

### Voir également

* class [SaveOptions](../saveoptions)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
