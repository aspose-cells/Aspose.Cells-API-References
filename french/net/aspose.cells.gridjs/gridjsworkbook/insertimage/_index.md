---
title: "GridJsWorkbook.InsertImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridJsWorkbook. Insère une image dans la feuille de calcul à partir d'un flux de fichier ou de l'URL ; soit le flux de fichier, soit l'URL doit être fourni, ou insère une forme lorsque p.type est l'un des AutoShapeType"
type: docs
url: /fr/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

Insère une image dans la feuille de calcul depuis le flux de fichier ou l'URL (le flux de fichier ou l'URL doit être fourni) ou insère une forme lorsque p.type est l'un des AutoShapeType.

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uid | String | L'identifiant unique pour le cache de fichiers |
| p | String | La chaîne au format JSON pour l'opération qui spécifie l'emplacement de la cellule, le nom de la feuille de calcul, la ligne supérieure gauche, la colonne supérieure gauche pour l'image, etc. {name:'sheet1',ri:1,ci:1} |
| s | Stream | Le flux de fichier de l'image |
| imageUrl | String | L'URL du fichier image |

### Valeur de retour

La chaîne au format JSON de l'image insérée

### Voir aussi

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


