---
title: Add
second_title: Aspose.Cells for .NET API Referansı
description: Veri kaynağı olarak PivotTable kullanarak yeni bir Zaman Çizelgesi ekleyin
type: docs
weight: 20
url: /tr/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Veri kaynağı olarak PivotTable kullanarak yeni bir Zaman Çizelgesi ekleyin

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| row | Int32 | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin satır dizini. |
| column | Int32 | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin sütun dizini. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField adı |

### Geri dönüş değeri

Yeni eklenen Zaman Çizelgesi dizini

### Örnekler

```csharp

[C#]
//PivotTable'ı veri kaynağı olarak kullanarak yeni bir Zaman Çizelgesi ekleyin
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* ad alanı [Aspose.Cells.Timelines](../../timelinecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Veri kaynağı olarak PivotTable kullanarak yeni bir Zaman Çizelgesi ekleyin

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Zaman Çizelgesi aralığının sol üst köşesindeki hücre adı. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField adı |

### Geri dönüş değeri

Yeni eklenen Zaman Çizelgesi dizini

### Örnekler

```csharp

[C#]
//PivotTable'ı veri kaynağı olarak kullanarak yeni bir Zaman Çizelgesi ekleyin
sheet.Timelines.Add(pivot, "i15", "date");
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* ad alanı [Aspose.Cells.Timelines](../../timelinecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Veri kaynağı olarak PivotTable kullanarak yeni bir Zaman Çizelgesi ekleyin

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| row | Int32 | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin satır dizini. |
| column | Int32 | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin sütun dizini. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField dizini |

### Geri dönüş değeri

Yeni eklenen Zaman Çizelgesi dizini

### Örnekler

```csharp

[C#]
//PivotTable'ı veri kaynağı olarak kullanarak yeni bir Zaman Çizelgesi ekleyin
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* ad alanı [Aspose.Cells.Timelines](../../timelinecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Veri kaynağı olarak PivotTable kullanarak yeni bir Zaman Çizelgesi ekleyin

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Zaman Çizelgesi aralığının sol üst köşesindeki hücre adı. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField dizini |

### Geri dönüş değeri

Yeni eklenen Zaman Çizelgesi dizini

### Örnekler

```csharp

[C#]
//PivotTable'ı veri kaynağı olarak kullanarak yeni bir Zaman Çizelgesi ekleyin
sheet.Timelines.Add(pivot, "i5", 1);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* ad alanı [Aspose.Cells.Timelines](../../timelinecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Veri kaynağı olarak PivotTable kullanarak yeni bir Zaman Çizelgesi ekleyin

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| row | Int32 | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin satır dizini. |
| column | Int32 | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin sütun dizini. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Geri dönüş değeri

Yeni eklenen Zaman Çizelgesi dizini

### Örnekler

```csharp

[C#]
//PivotTable'ı veri kaynağı olarak kullanarak yeni bir Zaman Çizelgesi ekleyin
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* ad alanı [Aspose.Cells.Timelines](../../timelinecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Veri kaynağı olarak PivotTable kullanarak yeni bir Zaman Çizelgesi ekleyin

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Zaman Çizelgesi aralığının sol üst köşesindeki hücre adı. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Geri dönüş değeri

Yeni eklenen Zaman Çizelgesi dizini

### Örnekler

```csharp

[C#]
//PivotTable'ı veri kaynağı olarak kullanarak yeni bir Zaman Çizelgesi ekleyin
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### Ayrıca bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* ad alanı [Aspose.Cells.Timelines](../../timelinecollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
