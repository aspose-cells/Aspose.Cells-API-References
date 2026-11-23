---
title: "Classe Config"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.Config. Représente tous les paramètres statiques pour GridJs"
type: docs
url: /fr/net/aspose.cells.gridjs/config/
---
## Config class

Représente tous les paramètres statiques pour GridJs.

```csharp
public class Config
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Config](config/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | Indique s'il faut ajuster automatiquement la largeur des colonnes lors du chargement du fichier. La valeur par défaut est `false`. Avertissement : définir cette valeur sur `true` effectuera une opération d'ajustement automatique de toutes les colonnes après le chargement, ce qui peut avoir un impact notable sur les performances. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | Indique s'il faut ajuster automatiquement la hauteur des lignes lors du chargement du fichier. La valeur par défaut est `false`. Avertissement : définir cette valeur sur `true` effectuera une opération d'ajustement automatique de toutes les lignes après le chargement, ce qui peut avoir un impact notable sur les performances. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Obtient/Définit s'il faut optimiser automatiquement les performances de chargement pour une feuille de calcul avec de grandes cellules. Cela ignorera certains styles /borders pour réduire le temps de chargement. La valeur par défaut est true. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | Obtient/definit le nom de la route de base pour l'URL du contrôleur GridJs. La valeur par défaut est "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | Obtient/Définit les PdfSaveOptions personnalisés pour l'exportation PDF. Si définies, elles seront utilisées à la place des options par défaut. La valeur par défaut est null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Obtient/Définit la colonne maximale par défaut pour une feuille de calcul vide. La valeur par défaut est 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Obtient/Définit la ligne maximale par défaut pour une feuille de calcul vide. La valeur par défaut est 12. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | Obtient/definit si le rendu des graphiques côté client est activé. Si défini sur false, GridJs reviendra uniquement aux images/formes de graphiques générées par le serveur. La valeur par défaut est true. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Obtient/Définit le répertoire de cache pour stocker le fichier de feuille de calcul. Nous devons le définir sur un chemin spécifique avant d'utiliser GridJs. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Obtient/Définit si l'on doit afficher la plage maximale qui comprend les données, le style, les cellules fusionnées et les formes. Si la dernière ligne ou colonne contient des cellules sans valeur ni formule mais avec un style personnalisé, alors nous n'afficherons pas cette ligne/colonne lorsque cette valeur est vraie. La valeur par défaut est vraie. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Obtient/Définit si la prise en charge de l'édition collaborative est activée, la valeur par défaut est false. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Obtient/Définit si la limitation du nombre total de formes/images affichées dans une feuille de calcul est activée, si réglé sur true, GridJs limitera le nombre total de formes ou d'images affichées dans une feuille de calcul à MaxShapeOrImageCount. La valeur par défaut est true. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | Obtient/definit si GridJs s'exécute à l'intérieur d'un hôte WebAssembly dans le navigateur au lieu d'un processus serveur. Lorsque true, aucun chemin FileCacheDirectory / disque / thread d'interruption n'est utilisé et le cache de fichiers doit provenir de GridJsOptions.CacheImp. GridJsOptions.IsWasm définit cela lors de la construction du service GridJs, de sorte qu'un seul Aspose.Cells.GridJs.dll sert les deux hôtes. La valeur par défaut est false. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | Obtient/Définit les options de configuration du cache JSON. Contrôle le comportement du cache mémoire (L1) et disque (L2) pour le JSON du classeur généré. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Obtient/Définit si l'on doit charger uniquement la feuille de calcul active, la valeur par défaut est false. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Obtient/Définit le nombre maximal de secondes d'expiration lors de l'enregistrement en PDF. La valeur par défaut est 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Obtient/Définit le nombre total de formes ou d'images affichées dans la feuille active, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Obtient/Définit la largeur ou hauteur maximale pour une forme ou une image, GridJs ignorera la forme ou l'image dont la largeur ou la hauteur dépasse cette valeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Obtient/Définit le nombre total de formes ou d'images affichées dans le classeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Obtient/Définit les destinations websocket préfixées par \"/topic\". La valeur par défaut est \"/topic/opr\". Utilisé uniquement en mode collaboratif. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Obtient/Définit le répertoire de cache pour les images. (cela prend effet lorsque GridJsWorkbook.CacheImp est null) Le chemin par défaut sera \"_piccache\" à l'intérieur du FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Obtient/Définit si l'on doit vérifier si les images ont la même source, la valeur par défaut est true. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Obtient/Définit si l'on doit enregistrer le fichier HTML en tant qu'archive zip, la valeur par défaut est false. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Obtient/Définit si la feuille de graphique doit être affichée. La valeur par défaut est false. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Obtient/Définit si l'on doit ignorer les formes invisibles pour l'UI, la valeur par défaut est true. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Obtient/Définit si l'on doit utiliser PageSetup.PrintArea pour la plage d'affichage UI lorsque la feuille possède un paramètre PageSetup pour PrintArea. La valeur par défaut est false. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Définit le dossier des polices |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Définit les dossiers de polices |

## Champs

| Nom | Description |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | Indique si l'on utilise un identifiant généré par le client au lieu de l'identifiant réel de la forme dans les opérations liées à la rédaction. |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


