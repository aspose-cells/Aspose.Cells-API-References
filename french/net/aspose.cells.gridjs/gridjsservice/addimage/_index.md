---
title: "GridJsService.AddImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridJsService. Applique l'ajout d'image depuis un fichier local, les octets du fichier proviennent de JS FormData ou de tout hôte."
type: docs
url: /fr/net/aspose.cells.gridjs/gridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Applique l'opération d'ajout d'image depuis un fichier local (les octets du fichier proviennent de JS FormData ou de tout hôte).

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

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Applique l'opération d'ajout d'image depuis un fichier local.

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

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


