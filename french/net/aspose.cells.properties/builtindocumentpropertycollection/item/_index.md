---
title: Item
second_title: Référence de l'API Aspose.Cells pour .NET
description: Renvoie unDocumentPropertyaspose.cells.properties/documentproperty objet par le nom de la propriété.
type: docs
weight: 110
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Renvoie un[`DocumentProperty`](../../documentproperty) objet par le nom de la propriété.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Paramètre | La description |
| --- | --- |
| name | Nom non sensible à la casse de la propriété à récupérer. |

### Remarques

Les noms de chaîne des propriétés correspondent aux noms des propriétés typed disponibles sur[`BuiltInDocumentPropertyCollection`](../../builtindocumentpropertycollection).

Si vous demandez une propriété qui n'est pas présente dans le document, mais que le nom de la propriété est reconnu comme un nom intégré valide, un nouveau[`DocumentProperty`](../../documentproperty) est créé, ajouté à la collection et renvoyé. La propriété nouvellement créée se voit attribuer une valeur par défaut (chaîne vide, zéro, faux ou DateTime.MinValue selon le type de la propriété intégrée).

Si vous demandez une propriété qui n'est pas présente dans le document et que le nom n'est pas reconnu comme un nom intégré, une valeur nulle est renvoyée.

### Voir également

* class [DocumentProperty](../../documentproperty)
* class [BuiltInDocumentPropertyCollection](../../builtindocumentpropertycollection)
* espace de noms [Aspose.Cells.Properties](../../builtindocumentpropertycollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
