---
title: Add
second_title: Aspose.Cells for .NET API Referansı
description: Veri kaynağı olarak PivotTable kullanarak yeni bir Dilimleyici ekleyin
type: docs
weight: 20
url: /tr/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Veri kaynağı olarak PivotTable kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Dilimleyici aralığının sol üst köşesindeki hücre. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField adı |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Veri kaynağı olarak PivotTable kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| row | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini. |
| column | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField adı |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Veri kaynağı olarak PivotTable kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| row | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini. |
| column | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField dizini |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Veri kaynağı olarak PivotTable kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Dilimleyici aralığının sol üst köşesindeki hücre. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField dizini |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Veri kaynağı olarak PivotTable kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| row | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini. |
| column | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Veri kaynağı olarak PivotTable kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Dilimleyici aralığının sol üst köşesindeki hücre. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| table | ListObject | ListObject nesnesi |
| index | Int32 | ListObject.ListColumns içindeki ListColumn dizini |
| destCellName | String | Dilimleyici aralığının sol üst köşesindeki hücre. |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### Ayrıca bakınız

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| table | ListObject | ListObject nesnesi |
| listColumn | ListColumn | ListObject.ListColumns içindeki ListColumn |
| destCellName | String | Dilimleyici aralığının sol üst köşesindeki hücre. |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### Ayrıca bakınız

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| table | ListObject | ListObject nesnesi |
| listColumn | ListColumn | ListObject.ListColumns içindeki ListColumn |
| row | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini. |
| column | Int32 | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini. |

### Geri dönüş değeri

Yeni ekle Dilimleyici dizini

### Örnekler

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### Ayrıca bakınız

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* ad alanı [Aspose.Cells.Slicers](../../slicercollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
