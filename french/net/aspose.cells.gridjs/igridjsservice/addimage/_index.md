---
title: "IGridJsService.AddImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IGridJsService. Applique l'opération d'ajout d'image depuis un fichier local en prenant directement les octets de l'image"
type: docs
url: /fr/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Applique l'opération d'ajout d'image depuis un fichier local, en prenant les octets de l'image directement.

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| p | String | Le paramètre de chaîne JSON |
| uid | String | L'identifiant unique pour le cache de fichier. |
| iscontrol | String | Spécifiez s'il s'agit d'un contrôle. |
| fileBytes | Byte[] | Les octets bruts du fichier image |

### Valeur de retour

Le résultat de chaîne JSON

### Voir aussi

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Applique l'opération d'ajout d'image depuis un fichier local, en prenant les fichiers de formulaire téléchargés.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| p | String | Le paramètre de chaîne JSON |
| uid | String | L'identifiant unique pour le cache de fichier. |
| iscontrol | String | Spécifiez s'il s'agit d'un contrôle. |
| fichiers | IFormFileCollection | Le fichier de formulaire de l'image |

### Valeur de retour

Le résultat de chaîne JSON

### Voir aussi

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


