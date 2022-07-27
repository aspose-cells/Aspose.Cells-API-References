---
title: Add
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajouter un nouveau segment en utilisant le tableau croisé dynamique comme source de données
type: docs
weight: 20
url: /fr/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Ajouter un nouveau segment en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage Slicer. |
| baseFieldName | String | Le nom de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Ajouter un nouveau segment en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer. |
| baseFieldName | String | Le nom de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Ajouter un nouveau segment en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer. |
| baseFieldIndex | Int32 | L'index de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Ajouter un nouveau segment en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage Slicer. |
| baseFieldIndex | Int32 | L'index de PivotField dans PivotTable.BaseFields |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Ajouter un nouveau segment en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer. |
| baseField | PivotField | Le champ croisé dynamique dans PivotTable.BaseFields |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Ajouter un nouveau segment en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivot | PivotTable | Objet tableau croisé dynamique |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage Slicer. |
| baseField | PivotField | Le champ croisé dynamique dans PivotTable.BaseFields |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### Voir également

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| table | ListObject | Objet ListObject |
| index | Int32 | L'index de ListColumn dans ListObject.ListColumns |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage Slicer. |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### Voir également

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| table | ListObject | Objet ListObject |
| listColumn | ListColumn | La ListColumn dans ListObject.ListColumns |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage Slicer. |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### Voir également

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| table | ListObject | Objet ListObject |
| listColumn | ListColumn | La ListColumn dans ListObject.ListColumns |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer. |

### Return_Value

Le nouvel index add Slicer

### Exemples

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### Voir également

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* espace de noms [Aspose.Cells.Slicers](../../slicercollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
