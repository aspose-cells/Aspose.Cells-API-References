---
title: "GridWorksheet.FreezePanes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridWorksheet méthode. Gèle les volets à la cellule spécifiée dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridworksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

Gèle les volets à la cellule spécifiée dans la feuille de calcul.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |
| freezedRows | Int32 | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | Int32 | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### Remarques

L'index de ligne et l'index de colonne ne peuvent pas tous deux être zéro. Le nombre de lignes et le nombre de colonnes ne peuvent pas non plus être tous deux zéro.

### Voir aussi

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

Gèle les volets à la cellule spécifiée dans la feuille de calcul.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| column | Int32 | Index de colonne. |
| freezedRows | Int32 | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | Int32 | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### Remarques

L'index de ligne et l'index de colonne ne peuvent pas tous deux être zéro. Le nombre de lignes et le nombre de colonnes ne peuvent pas non plus être tous deux zéro.

Les deux premiers paramètres spécifient la position gelée et les deux derniers paramètres spécifient la zone gelée sur le volet supérieur gauche.

### Voir aussi

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


