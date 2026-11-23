---
title: "Interface IGridJsService"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.GridJs.IGridJsService. Représente l'interface des API d'opérations de base utilisées dans les actions du contrôleur."
type: docs
url: /fr/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

Représente l'interface des API d'opération de base utilisées dans les actions du contrôleur.

```csharp
public interface IGridJsService : IDisposable
```

## Méthodes

| Nom | Description |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | Applique l'opération d'ajout d'image depuis un fichier local, en prenant les octets de l'image directement. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Applique l'opération d'ajout d'image depuis un fichier local, en prenant les fichiers de formulaire téléchargés. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | Applique l'opération d'ajout d'image depuis une URL distante. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Vérifie si l'instance du classeur est dans le cache mémoire. Cette méthode s'applique uniquement au mode collaboratif. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | Efface toutes les entrées du cache JSON (mémoire et disque). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | Efface toutes les entrées du cache JSON appartenant à l'ID unique spécifié. Appelez ceci après avoir modifié le fichier source hors bande afin que la prochaine requête régénère le JSON. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Applique l'opération de copie d'image. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Obtient la chaîne JSON du fichier par l'ID unique spécifié. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Obtient la chaîne JSON du classeur par l'ID unique spécifié. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Écrit la chaîne JSON du classeur dans le flux |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Écrit la chaîne JSON du classeur dans le flux |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Écrit la chaîne JSON du fichier dans le flux par l'ID unique spécifié. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Écrit la chaîne JSON du classeur dans le flux par l'ID unique spécifié. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Applique l'opération de téléchargement du fichier |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Obtenir le flux du fichier |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | Obtient le rappel d'avertissement personnalisé pour l'importation du fichier. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Obtenir le flux de l'image. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Obtient l'URL de l'image. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Écrit la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié dans le flux. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Obtient la chaîne JSON du fichier depuis le cache en utilisant l'ID unique spécifié, définit le nom de fichier de sortie dans le JSON. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Obtient les données du tableau d'octets de l'objet OLE intégré. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | Définit le rappel d'avertissement personnalisé pour l'importation du fichier. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Applique l'opération de mise à jour. |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


