---
title: "GridValidationCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridValidationCollection. Ajoute un GridValidation à la collection. La validation est appliquée à la cellule spécifiée."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridvalidationcollection/add/
---
## Add(string) {#add_1}

Ajoute un [`GridValidation`](../../gridvalidation/) à la collection. La validation est appliquée à la cellule spécifiée.

```csharp
public GridValidation Add(string cellname)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellname | String | le nom de la cellule. |

### Valeur de retour

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Voir aussi

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int) {#add}

Ajoute un [`GridValidation`](../../gridvalidation/) à la collection. La validation est appliquée à la cellule spécifiée.

```csharp
public GridValidation Add(int row, int col)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de la cellule. |
| col | Int32 | Indice de colonne de la cellule. |

### Valeur de retour

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Voir aussi

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, bool, string) {#add_5}

Ajoute une validation à une cellule spécifiée par son nom.

```csharp
public void Add(string cellName, bool isRequired, string regEx)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule de grille. |
| isRequired | Boolean | Valeur indiquant si la valeur de la cellule est requise. |
| regEx | String | Expression régulière. |

### Voir aussi

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, ICustomValidation) {#add_2}

Ajoute une validation à une cellule spécifiée à l'index de ligne et de colonne.

```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de la cellule. |
| col | Int32 | Indice de colonne de la cellule. |
| customValidation | ICustomValidation | Objet de validation personnalisé. |

### Voir aussi

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, bool, string) {#add_3}

Ajoute une validation à une cellule spécifiée à l'index de ligne et de colonne.

```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de la cellule. |
| col | Int32 | Indice de colonne de la cellule. |
| isRequired | Boolean | Valeur indiquant si la valeur de la cellule est requise. |
| regEx | String | Expression régulière. |

### Voir aussi

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, ICustomValidation) {#add_4}

Ajoute une validation à une cellule spécifiée par son nom.

```csharp
public void Add(string cellName, ICustomValidation customValidation)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule de grille. |
| customValidation | ICustomValidation | Objet de validation personnalisé. |

### Voir aussi

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


