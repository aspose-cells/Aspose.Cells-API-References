---
title: CultureCustom
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtient et définit la chaîne de modèle dépendant de la culture pour le format de nombre. Si aucun format de nombre na été défini pour cet objet null sera renvoyé. Si le format de nombre est intégré la chaîne de modèle correspondant au nombre intégré sera renvoyée.
type: docs
weight: 50
url: /fr/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Obtient et définit la chaîne de modèle dépendant de la culture pour le format de nombre. Si aucun format de nombre n'a été défini pour cet objet, null sera renvoyé. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée.

```csharp
public string CultureCustom { get; set; }
```

### Remarques

Pour le format de nombre intégré, à la fois le contenu du modèle (par exemple, un format de date intégré est "m/d/y" pour certains paramètres régionaux, mais pour certains autres paramètres régionaux, il devient "d/m/y") et le spécificateur de format (par exemple, certains paramètres régionaux utilisent un caractère autre que 'y' pour représenter la partie année pour le formatage de la date) dépendent de la culture ; Pour le format personnalisé spécifié par l'utilisateur, seuls les spécificateurs de format sont modifiés en fonction de la culture, autres parties du modèle de formatage ne sera pas modifié.

### Voir également

* class [Style](../../style)
* espace de noms [Aspose.Cells](../../style)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
