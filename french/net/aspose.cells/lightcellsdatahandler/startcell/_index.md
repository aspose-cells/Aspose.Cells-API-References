---
title: StartCell
second_title: Référence de l'API Aspose.Cells pour .NET
description: Se prépare à traiter une cellule.
type: docs
weight: 30
url: /fr/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Se prépare à traiter une cellule.

```csharp
public bool StartCell(int columnIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| columnIndex | Int32 | index de colonne de la cellule à traiter |

### Return_Value

si cette cellule doit être traitée. false pour ignorer la cellule et vérifier la suivante jusqu'à atteindre la fin des données des cellules de la ligne actuelle

### Remarques

Il sera appelé lorsqu'il atteindra une cellule existante dans la ligne actuelle. La ligne actuelle est la ligne du dernier appel de[`ProcessRow`](../processrow) .

### Voir également

* interface [LightCellsDataHandler](../../lightcellsdatahandler)
* espace de noms [Aspose.Cells](../../lightcellsdatahandler)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
