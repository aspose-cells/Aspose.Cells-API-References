---
title: "GridCells.DeleteRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridCells méthode. Supprime plusieurs lignes"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Supprime plusieurs lignes.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | L'index de la première ligne à supprimer. |
| totalRows | Int32 | Nombre de lignes à supprimer. |

### Remarques

Si la plage supprimée contient la partie supérieure (pas la totalité) du tableau (ListObject), la plage ne peut pas être supprimée et aucune action ne sera effectuée. Cela fonctionne comme MS Excel.

### Voir aussi

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

Supprime plusieurs lignes dans la feuille de calcul.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |
| totalRows | Int32 | Nombre de lignes à supprimer. |
| updateReference | Boolean | Indique si les références sont mises à jour dans d'autres feuilles de calcul. |

### Voir aussi

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


