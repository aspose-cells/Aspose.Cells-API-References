---
title: "PivotCache.CreatePivotTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotCache. Crée un rapport PivotTable sur une nouvelle feuille."
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

Crée un rapport PivotTable sur une nouvelle feuille.

```csharp
public PivotTable CreatePivotTable()
```

### Valeur de retour

L'objet PivotTable

### Remarques

L'appel de cette méthode créera un objet PivotTable et une nouvelle feuille de calcul. Ensuite, il ajoute l'objet PivotTable à la dernière position de GridWeb.Worksheets.PivotTables. Si vous appelez la méthode PivotTable.DataBind(), le rapport PivotTable sera rendu sur la feuille de calcul créée.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

Crée un rapport PivotTable sur une nouvelle feuille. Le nom de l'objet pivotTable

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### Valeur de retour

L'objet PivotTable

### Remarques

L'appel de cette méthode créera un objet PivotTable et une nouvelle feuille de calcul. Ensuite, il ajoute l'objet PivotTable à la dernière position de GridWeb.Worksheets.PivotTables. Si vous appelez la méthode PivotTable.DataBind(), le rapport PivotTable sera rendu sur la feuille de calcul créée.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

Crée un rapport PivotTable sur la feuille cible.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| targetSheet | WebWorksheet | La feuille sur laquelle le rapport pivotTable sera peint. |
| targetCell | WebCell | La cellule de départ sur laquelle le rapport pivotTable sera peint. |

### Valeur de retour

L'objet PivotTable

### Remarques

L'appel de cette méthode créera un objet PivotTable puis ajoutera l'objet PivotTable à la dernière position de GridWeb.Worksheets.PivotTables. Si vous appelez la méthode PivotTable.DataBind(), le rapport PivotTable sera rendu sur targetSheet à partir de targetCell.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

Crée un rapport PivotTable sur la feuille cible.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| targetSheet | WebWorksheet | La feuille sur laquelle le rapport pivotTable sera peint. |
| targetCell | WebCell | La cellule de départ sur laquelle le rapport pivotTable sera peint. |
| tableName | String | Le nom de l'objet pivotTable |

### Valeur de retour

L'objet PivotTable

### Remarques

L'appel de cette méthode créera un objet PivotTable nommé tableName, puis ajoutera l'objet PivotTable à la dernière position de GridWeb.Worksheets.PivotTables. Si vous appelez la méthode PivotTable.DataBind(), le rapport PivotTable sera rendu sur targetSheet à partir de targetCell.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


