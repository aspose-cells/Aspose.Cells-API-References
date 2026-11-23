---
title: "Classe GridJsService"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.GridJsService. Fournit les API d'opérations de base utilisées dans les actions du contrôleur"
type: docs
url: /fr/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Fournit les API d'opération de base utilisées dans les actions du contrôleur.

```csharp
public class GridJsService : IGridJsService
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | Le constructeur de GridJsService pour les hôtes qui construisent eux‑mêmes l'objet d'options (l'hôte navigateur WASM et toute configuration serveur non‑DI). |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | Le constructeur par défaut de GridJsService |

## Propriétés

| Nom | Description |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Représente les paramètres du classeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | Applique l'opération d'ajout d'image depuis un fichier local (les octets du fichier proviennent de JS FormData ou de tout hôte). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Applique l'opération d'ajout d'image depuis un fichier local. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Applique l'opération d'ajout d'image depuis une URL distante. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Vérifie si l'instance du classeur est dans le cache mémoire. Cette méthode s'applique uniquement au mode collaboratif. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | Efface toutes les entrées du cache JSON (mémoire et disque). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | Efface toutes les entrées du cache JSON appartenant à l'ID unique spécifié. Appelez ceci après avoir modifié le fichier source hors bande afin que la prochaine requête régénère le JSON. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Applique l'opération de copie d'image. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | Cette méthode est uniquement pour Java, elle implémente la méthode destroy dans DisposableBean, qui sera appelée automatiquement par Spring à la fin de la requête ; en réalité elle appellera la méthode Dispose. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Obtient la chaîne JSON du fichier par l'ID unique spécifié. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Obtient la chaîne JSON du classeur par l'ID unique spécifié. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Écrit la chaîne JSON du fichier dans le flux. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Écrit la chaîne JSON du classeur dans le flux |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Écrit la chaîne JSON du fichier dans le flux par l'ID unique spécifié. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Écrit la chaîne JSON du classeur dans le flux par l'ID unique spécifié. |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | Effectue des tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Applique l'opération de téléchargement du fichier |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Obtenir le flux du fichier |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | Obtient le rappel d'avertissement personnalisé pour l'importation du fichier. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Obtenir le flux de l'image. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Obtient l'URL de l'image. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Écrit la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié dans le flux. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Obtient la chaîne JSON du fichier depuis le cache en utilisant l'ID unique spécifié, définit le nom de fichier de sortie dans le JSON. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Obtient les données du tableau d'octets de l'objet OLE intégré. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | Définit le rappel d'avertissement personnalisé pour l'importation du fichier. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Traduire toutes les valeurs de chaîne vers la langue cible dans la feuille de calcul. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Applique l'opération de mise à jour. |

### Voir aussi

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


