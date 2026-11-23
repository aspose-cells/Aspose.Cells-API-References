---
title: "GridWorksheet.CreateSubtotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridWorksheet. Crée un sous‑total dans la feuille"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## CreateSubtotal(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) {#createsubtotal_1}

Crée un sous-total dans la feuille.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | Int32 | L'index de ligne de la ligne de nom de colonne. |
| dataRows | Int32 | Le nombre de lignes de données. |
| groupByColumnIndex | Int32 | L'index de colonne de la colonne à regrouper. |
| subtotalFunction | SubtotalFunction | Le type de fonction de sous-total. |
| subtotalColumnIndexList | Int32[] | Les index de colonnes à sous-totaliser. |
| functionLabel | String | L'étiquette de la fonction de sous-total. |
| grandCellStyle | GridTableItemStyle | Le style de la ligne du total général. |
| subtotalCellStyle | GridTableItemStyle | Le style de la ligne de sous-total. |
| numberType | NumberType | Le type de nombre des cellules de résultat du sous-total. |
| customString | String | La chaîne de format personnalisée des cellules de résultat du sous-total. Peut être nulle. |

### Voir aussi

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreateSubtotal(int, int, int, SubtotalFunction, int[]) {#createsubtotal}

Crée un sous-total dans la feuille.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | Int32 | L'index de ligne de la ligne de nom de colonne. |
| dataRows | Int32 | Le nombre de lignes de données. |
| groupByColumnIndex | Int32 | L'index de colonne de la colonne à regrouper. |
| subtotalFunction | SubtotalFunction | Le type de fonction de sous-total. |
| subtotalColumnIndexList | Int32[] | Les index de colonnes à sous-totaliser. |

### Voir aussi

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


