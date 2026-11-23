---
title: "Classe GridPdfSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridDesktop.Data.GridPdfSaveOptions classe. Représente les options pour enregistrer un fichier PDF."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/
---
## GridPdfSaveOptions class

Représente les options d'enregistrement d'un fichier PDF.

```csharp
public class GridPdfSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridPdfSaveOptions](gridpdfsaveoptions/)() | Le constructeur de GridSaveOptions |

## Propriétés

| Nom | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cachedfilefolder/) { get; set; } | Le dossier de fichiers en cache est utilisé pour stocker de grandes données. |
| [CalculateFormula](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/calculateformula/) { get; set; } | Indique s'il faut calculer les formules avant d'enregistrer le fichier pdf. |
| [ClearData](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l'enregistrement du fichier. |
| [Compliance](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/compliance/) { get; set; } | La conversion du classeur en PDF se fera selon le PdfCompliance de cette propriété. |
| [CreateDirectory](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant l'enregistrement du fichier. |
| [CreatedTime](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdtime/) { get; set; } | Obtient et définit l'heure de génération du document pdf. |
| [CustomPropertiesExport](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/custompropertiesexport/) { get; set; } | Obtient ou définit une valeur déterminant la façon dont les données sont exportées vers le fichier PDF. La valeur par défaut est None. |
| [DisplayDocTitle](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/displaydoctitle/) { get; set; } | Indique si la barre de titre de la fenêtre doit afficher le titre du document. |
| [EmbedStandardWindowsFonts](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True pour intégrer les polices TrueType. N'affecte que les caractères ASCII 32-127. Les polices pour les codes de caractères supérieurs à 127 sont toujours intégrées. Les polices sont toujours intégrées pour les normes PDF/A-1a, PDF/A-1b. La valeur par défaut est true. |
| [EmfRenderSetting](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/emfrendersetting/) { get; set; } | Paramètre pour le rendu du métafichier Emf. |
| [ExportDocumentStructure](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/exportdocumentstructure/) { get; set; } | Indique s'il faut exporter la structure du document. |
| [FontEncoding](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/fontencoding/) { get; set; } | Obtient ou définit l'encodage des polices intégrées dans le pdf. |
| [MergeAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/mergeareas/) { get; set; } | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant l'enregistrement du fichier. |
| [OptimizationType](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/optimizationtype/) { get; set; } | Obtient et définit le type d'optimisation du pdf. |
| [PdfCompression](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/pdfcompression/) { get; set; } | Indique l'algorithme de compression |
| [Producer](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/producer/) { get; set; } | Obtient et définit le producteur du document pdf généré. |
| [RefreshChartCache](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/refreshchartcache/) { get; set; } | Indique si le rafraîchissement des données du cache du graphique est activé. |
| [SortExternalNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortexternalnames/) { get; set; } | Indique si le tri des noms définis externes doit être effectué avant d'enregistrer le fichier. |
| [SortNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortnames/) { get; set; } | Indique si le tri des noms définis doit être effectué avant d'enregistrer le fichier. |
| [UpdateSmartArt](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/updatesmartart/) { get; set; } | Indique si la mise à jour du paramètre SmartArt est activée. La valeur par défaut est false. |
| [ValidateMergedAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/validatemergedareas/) { get; set; } | Indique si la validation des cellules fusionnées doit être effectuée avant d'enregistrer le fichier. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetImageResample](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/)(int, int) | Définit le PPI (pixels par pouce) souhaité pour le rééchantillonnage des images et la qualité JPEG. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié, et les images dont le PPI dépasse le PPI spécifié (pixels par pouce) seront rééchantillonnées. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


