---
title: Add
second_title: Справочник по Aspose.Cells для .NET API
description: Добавить новый слайсер используя сводную таблицу в качестве источника данных
type: docs
weight: 20
url: /ru/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Добавить новый слайсер, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Добавить новый слайсер, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона слайсера. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Добавить новый слайсер, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона слайсера. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Добавить новый слайсер, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Добавить новый слайсер, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона слайсера. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |
| baseField | PivotField | Сводное поле в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Добавить новый слайсер, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Ячейка в верхнем левом углу диапазона среза. |
| baseField | PivotField | Сводное поле в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Добавить новый слайсер, используя ListObjet в качестве источника данных

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| table | ListObject | ListObject object |
| index | Int32 | Индекс ListColumn в ListObject.ListColumns |
| destCellName | String | Ячейка в верхнем -левый угол диапазона Slicer. |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### Смотрите также

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Добавить новый слайсер, используя ListObjet в качестве источника данных

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | ListColumn в ListObject.ListColumns |
| destCellName | String | Ячейка в левом верхнем углу угол диапазона Slicer. |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### Смотрите также

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Добавить новый слайсер, используя ListObjet в качестве источника данных

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | ListColumn в ListObject.ListColumns |
| row | Int32 | Индекс строки ячейки в верхний левый угол диапазона Slicer. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона среза. |

### Возвращаемое значение

Новый добавленный индекс слайсера

### Примеры

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### Смотрите также

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* пространство имен [Aspose.Cells.Slicers](../../slicercollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
