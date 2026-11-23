---
title: "Classe GridJsWorkbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.GridJsWorkbook. Représente la classe principale d'entrée pour GridJs"
type: docs
url: /fr/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Représente la classe principale d'entrée pour GridJs

```csharp
public class GridJsWorkbook
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | Crée une nouvelle instance de GridJsWorkbook. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | Obtient/Définit le répertoire de cache pour le stockage du fichier de feuille de calcul. Si cela n'est pas défini, nous utiliserons la propriété statique de [`FileCacheDirectory`](../config/filecachedirectory/) ou de [`CacheImp`](./cacheimp/). |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Représente les paramètres du classeur. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement pour l'importation du fichier. |

## Méthodes

| Nom | Description |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | Applique (exécute) toutes les opérations de rédaction dans le classeur en supprimant les formes de rédaction et leurs formes cibles ou en effaçant le contenu des plages de cellules cibles. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Vérifie si l'instance du classeur est dans le cache mémoire. Cette méthode s'applique uniquement au mode collaboratif. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | Effacer tout le cache JSON |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | Effacer le cache JSON selon l'uid (utilisé pour les scénarios comme UpdateCell où seul l'uid est disponible) |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Copie l'image ou la forme. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | Effectue des tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Obtient la chaîne du message d'erreur au format JSON. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Obtient la chaîne JSON à partir des données en mémoire, le nom de fichier par défaut dans le JSON est : book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Obtient la chaîne JSON à partir des données en mémoire, définit le nom de fichier de sortie dans le JSON. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | Obtient la chaîne JSON à partir des données en mémoire, définit le nom de fichier de sortie dans le JSON. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Obtient la chaîne JSON du fichier depuis le cache en utilisant l'ID unique spécifié, définit le nom de fichier de sortie dans le JSON. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Obtient les données du tableau d'octets de l'objet OLE intégré. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | Obtenir le JSON de la feuille spécifiée (avec cache) |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | Obtenir le JSON complet du classeur (avec cache) |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Importe le fichier Excel depuis le chemin d'accès. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Importe le fichier Excel depuis l'objet Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Importe le fichier Excel depuis le flux de fichier avec le format de chargement. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Importe le fichier Excel depuis le chemin d'accès. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Importe le fichier Excel depuis l'objet Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Importe le fichier Excel depuis le flux de fichier avec le format de chargement et le mot de passe d'ouverture. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Importe le fichier Excel depuis le flux de fichier. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Importe le fichier Excel depuis le chemin d'accès et le mot de passe d'ouverture. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importe le fichier Excel depuis le flux de fichier avec le format de chargement et le mot de passe d'ouverture. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Importe le fichier Excel depuis une chaîne au format JSON. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Insère une image dans la feuille de calcul depuis le flux de fichier ou l'URL (le flux de fichier ou l'URL doit être fourni) ou insère une forme lorsque p.type est l'un des AutoShapeType. |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | Génère le JSON à partir du classeur en mémoire et l'écrit dans le flux spécifié. Met éventuellement en cache le JSON généré pour une récupération ultérieure plus rapide. Principales différences avec JsonToStreamByUid : - Cette méthode utilise l'état actuel du classeur en mémoire (champ wb) - JsonToStreamByUid recharge le classeur à partir des fichiers de cache .cells sur le disque - Utilisez cette méthode lorsque vous souhaitez exporter l'état actuel du classeur après des modifications - Utilisez JsonToStreamByUid lorsque vous devez régénérer le JSON à partir d'un état de fichier précédemment mis en cache. Comportement de mise en cache (lorsqu'un uid est fourni) : - Vérifie le cache JSON avant de générer (mémoire L1 + disque L2) - En cas d'absence de cache, génère le JSON à partir du classeur en mémoire - Stocke le JSON généré dans le cache pour les requêtes futures |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON, et l'écrit dans le flux. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Récupère la chaîne JSON de la feuille spécifiée du fichier depuis le cache en utilisant l'identifiant unique spécifié, et l'écrit dans le flux. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Applique une mise à jour par lot aux données en mémoire. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | Effectue une rédaction sur un fichier Excel basée sur un tableau d'opérations JSON. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Enregistre les données en mémoire dans le fichier de cache avec le nom de fichier spécifié et définit également le mot de passe d'ouverture, le format d'enregistrement est basé sur l'extension du nom de fichier. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Enregistre les données en mémoire dans le sream, basé sur le format du fichier d'origine. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Enregistre les données en mémoire dans le chemin d'accès du fichier, si le fichier a une extension, le format d'enregistrement est basé sur l'extension du fichier. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Enregistre les données en mémoire dans le sream, le format d'enregistrement est html. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Enregistre les données en mémoire dans le chemin d'accès du fichier, le format d'enregistrement est html. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Enregistre les données en mémoire dans le sream, le format d'enregistrement est pdf. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Enregistre les données en mémoire dans le chemin d'accès du fichier, le format d'enregistrement est pdf. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Enregistre les données en mémoire dans le sream, le format d'enregistrement est xlsx. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Enregistre les données en mémoire dans le chemin d'accès du fichier, le format d'enregistrement est xlsx. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Définit InterruptMonitor pour l'opération de chargement. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Définit InterruptMonitor pour l'opération d'enregistrement. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | Définit la transparence des formes de rédaction dans le classeur. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Traduire toutes les valeurs de chaîne vers la langue cible dans la feuille de calcul. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Applique l'opération de mise à jour. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Obtient le format de chargement par extension de fichier |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | Obtenir le flux de l'image. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Obtient l'URL de l'image. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Génère un nouvel identifiant unique pour le cache de fichiers en utilisant le nom de fichier fourni. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Définissez l'URL de l'action de récupération de l'image de base depuis le contrôleur. |

## Champs

| Nom | Description |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Implémentation personnalisée pour le stockage du cache. Si vous souhaitez stocker le cache sous forme de flux, vous devez le configurer et l'implémenter. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Implémentation personnalisée pour le moteur de calcul. Si vous souhaitez effectuer un calcul personnalisé, vous devez le configurer et l'implémenter. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | valeur constante pour le type de l'image |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Obtient/Définit le moniteur de mise à jour pour suivre l'opération de mise à jour |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


