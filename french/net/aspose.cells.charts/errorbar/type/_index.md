---
title: Type
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente le type de montant de la barre derreur.
type: docs
weight: 60
url: /fr/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Représente le type de montant de la barre d'erreur.

```csharp
public ErrorBarType Type { get; set; }
```

### Exemples

```csharp
[C#]
// Définit le type de barre d'erreur personnalisé
aseries.YErrorBar.Type = ErrorBarType.InnerCustom;
aseries.YErrorBar.PlusValue = "=Sheet1!A1";
aseries.YErrorBar.MinusValue = "=Sheet1!A2";

[Visual Basic]
'Définit le type de barre d'erreur personnalisé
aseries.YErrorBar.Type = ErrorBarType.InnerCustom
aseries.YErrorBar.PlusValue = "=Sheet1!A1"
aseries.YErrorBar.MinusValue = "=Sheet1!A2"
```

### Voir également

* enum [ErrorBarType](../../errorbartype)
* class [ErrorBar](../../errorbar)
* espace de noms [Aspose.Cells.Charts](../../errorbar)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->