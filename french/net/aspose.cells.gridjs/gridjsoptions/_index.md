---
title: "Classe GridJsOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.GridJsOptions. Représente toutes les options de chargement pour GridJs"
type: docs
url: /fr/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

Représente toutes les options de chargement pour GridJs

```csharp
public class GridJsOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | Indique s'il faut ajuster automatiquement la largeur des colonnes lors du chargement du fichier, la valeur par défaut est false. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Indique s'il faut ajuster automatiquement la hauteur des lignes lors du chargement du fichier, la valeur par défaut est false. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Obtient/Définit s'il faut optimiser automatiquement les performances de chargement pour une feuille de calcul avec de grandes cellules. Cela ignorera certains styles /borders pour réduire le temps de chargement. La valeur par défaut est true. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | Obtient/Définit le nom de base de l'URL de route pour le contrôleur GridJs. La valeur par défaut est GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | Obtient/Définit les PdfSaveOptions personnalisés pour l'exportation PDF. Si définies, elles seront utilisées à la place des options par défaut. La valeur par défaut est null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Obtient/Définit la colonne maximale par défaut pour une feuille de calcul vide. La valeur par défaut est 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Obtient/Définit la ligne maximale par défaut pour une feuille de calcul vide. La valeur par défaut est 12. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | Obtient/Définit s'il faut activer le rendu de graphiques côté client. Si défini sur false, GridJs n'émettra que des images/formes de graphiques et ne nécessitera pas de rendu côté client. La valeur par défaut est true. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Obtient/Définit le répertoire de cache pour stocker le fichier de feuille de calcul. Nous devons le définir sur un chemin spécifique avant d'utiliser GridJs. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Obtient/Définit les dossiers de polices pour les polices dans les images/formes rendues. |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Obtient/Définit si l'on doit afficher la plage maximale qui comprend les données, le style, les cellules fusionnées et les formes. Si la dernière ligne ou colonne contient des cellules sans valeur ni formule mais avec un style personnalisé, alors nous n'afficherons pas cette ligne/colonne lorsque cette valeur est vraie. La valeur par défaut est vraie. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Obtient/Définit si la prise en charge de l'édition collaborative est activée, la valeur par défaut est false. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Obtient/Définit si la limitation du nombre total de formes/images affichées dans une feuille de calcul est activée, si réglé sur true, GridJs limitera le nombre total de formes ou d'images affichées dans une feuille de calcul à MaxShapeOrImageCount. La valeur par défaut est true. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | Obtient/Définit si GridJs s'exécute à l'intérieur d'un hôte WebAssembly de navigateur au lieu d'un processus serveur. Lorsque true, aucun chemin FileCacheDirectory / disque / thread d'interruption n'est utilisé, et le cache de fichiers doit provenir de CacheImp, car un hôte navigateur n'a pas de disque local. Il sélectionne les chemins de code à l'exécution, de sorte qu'un seul Aspose.Cells.GridJs.dll sert les deux hôtes. La valeur par défaut est false. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | Obtient/Définit les options de configuration du cache JSON. Contrôle le comportement du cache mémoire (L1) et disque (L2) pour le JSON du classeur généré. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Obtient/Définit si l'on doit charger uniquement la feuille de calcul active, la valeur par défaut est false. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Obtient/Définit le nombre maximal de secondes d'expiration lors de l'enregistrement en PDF. La valeur par défaut est 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Obtient/Définit le nombre total de formes ou d'images affichées dans la feuille active, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Obtient/Définit la largeur ou hauteur maximale pour une forme ou une image, GridJs ignorera la forme ou l'image dont la largeur ou la hauteur dépasse cette valeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Obtient/Définit le nombre total de formes ou d'images affichées dans le classeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Obtient/Définit les destinations websocket préfixées par \"/topic\". La valeur par défaut est \"/topic/opr\". Utilisé uniquement en mode collaboratif. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Obtient/Définit le répertoire de cache pour les images. (cela prend effet lorsque GridJsWorkbook.CacheImp est null) Le chemin par défaut sera \"_piccache\" à l'intérieur du FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Obtient/Définit si l'on doit vérifier si les images ont la même source, la valeur par défaut est true. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Obtient/Définit si l'on doit enregistrer le fichier HTML en tant qu'archive zip, la valeur par défaut est false. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Obtient/Définit si la feuille de graphique doit être affichée. La valeur par défaut est false. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Obtient/Définit si l'on doit ignorer les formes invisibles pour l'UI, la valeur par défaut est true. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Obtient/Définit si l'on doit utiliser PageSetup.PrintArea pour la plage d'affichage UI lorsque la feuille possède un paramètre PageSetup pour PrintArea. La valeur par défaut est false. |

## Champs

| Nom | Description |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Implémentation personnalisée pour le stockage du cache. Si vous souhaitez stocker le cache sous forme de flux, vous devez le définir et l'implémenter. Un hôte WebAssembly (IsWasm = true) doit le définir, car il n'y a pas de disque local pour le cache de fichiers par défaut. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | Indique si l'on utilise un identifiant généré par le client au lieu de l'identifiant réel de la forme dans les opérations liées à la rédaction. |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


