---
title: Clear
second_title: Référence de l'API Aspose.Cells pour .NET
description: Supprime tous les liens externes.
type: docs
weight: 40
url: /fr/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Supprime tous les liens externes.

```csharp
public void Clear()
```

### Remarques

Lors de la suppression de liens externes, toutes les formules qui y font référence seront également supprimées car les références deviennent invalides.

### Voir également

* class [ExternalLinkCollection](../../externallinkcollection)
* espace de noms [Aspose.Cells](../../externallinkcollection)
* Assemblée [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Supprime tous les liens externes.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Indique si toutes les références de liens externes sont mises à jour en tant que références du classeur en cours lui-même. |

### Remarques

Si les références doivent être mises à jour, les références aux liens externes dans les formules seront remplacées par le classeur actuel. Par exemple, la formule d'origine d'une cellule est "='externalsource.xlam'!customfunction()", après la suppression des liens externes, la formule deviendra "=customfunction()". Si les références ne doivent pas être mises à jour, toutes les formules avec des références à des liens externes seront également supprimées car ces références deviennent invalides.

### Voir également

* class [ExternalLinkCollection](../../externallinkcollection)
* espace de noms [Aspose.Cells](../../externallinkcollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
