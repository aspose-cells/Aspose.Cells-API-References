---
title: Add
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
type: docs
weight: 20
url: /fr/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseFieldName | String | Le nom de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index d'ajout de chronologie

### Exemples

```csharp

[C#]
//Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espace de noms [Aspose.Cells.Timelines](../../timelinecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| destCellName | String | Le nom de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseFieldName | String | Le nom de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index d'ajout de chronologie

### Exemples

```csharp

[C#]
//Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
sheet.Timelines.Add(pivot, "i15", "date");
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espace de noms [Aspose.Cells.Timelines](../../timelinecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseFieldIndex | Int32 | L'index de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index d'ajout de chronologie

### Exemples

```csharp

[C#]
//Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espace de noms [Aspose.Cells.Timelines](../../timelinecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| destCellName | String | Le nom de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseFieldIndex | Int32 | L'index de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index d'ajout de chronologie

### Exemples

```csharp

[C#]
//Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
sheet.Timelines.Add(pivot, "i5", 1);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espace de noms [Aspose.Cells.Timelines](../../timelinecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseField | PivotField | Le champ croisé dynamique dans PivotTable.BaseFields |

### Return_Value

Le nouvel index d'ajout de chronologie

### Exemples

```csharp

[C#]
//Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* espace de noms [Aspose.Cells.Timelines](../../timelinecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| destCellName | String | Le nom de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseField | PivotField | Le champ croisé dynamique dans PivotTable.BaseFields |

### Return_Value

Le nouvel index d'ajout de chronologie

### Exemples

```csharp

[C#]
//Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* espace de noms [Aspose.Cells.Timelines](../../timelinecollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
