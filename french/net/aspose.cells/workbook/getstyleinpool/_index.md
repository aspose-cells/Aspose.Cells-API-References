---
title: GetStyleInPool
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtient le style dans le pool de styles. Tous les styles du classeur seront rassemblés dans un pool. Il ny a quun simple index de référence dans les cellules.
type: docs
weight: 450
url: /fr/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Obtient le style dans le pool de styles. Tous les styles du classeur seront rassemblés dans un pool. Il n'y a qu'un simple index de référence dans les cellules.

```csharp
public Style GetStyleInPool(int index)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| index | Int32 | L'index. |

### Return_Value

Le style dans le pool correspond à l'index donné, peut être nul.

### Remarques

Si le style renvoyé est modifié, le style de toutes les cellules (qui fait référence à ce style) sera modifié.

### Voir également

* class [Style](../../style)
* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
