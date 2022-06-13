---
title: Add
second_title: Справочник по Aspose.Cells для .NET API
description: Добавить новую временную шкалу используя сводную таблицу в качестве источника данных
type: docs
weight: 20
url: /ru/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона временной шкалы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона временной шкалы. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс временной шкалы

### Примеры

```csharp

[C#]
  //Добавить новую временную шкалу, используя сводную таблицу в качестве данных source
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* пространство имен [Aspose.Cells.Timelines](../../timelinecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Имя ячейки в верхнем левом углу диапазона временной шкалы. |
| baseFieldName | String | Имя PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс временной шкалы

### Примеры

```csharp

[C#]
  //Добавить новую временную шкалу, используя сводную таблицу в качестве данных source
sheet.Timelines.Add(pivot, "i15", "date");
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* пространство имен [Aspose.Cells.Timelines](../../timelinecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона временной шкалы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона временной шкалы. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс временной шкалы

### Примеры

```csharp

[C#]
  //Добавить новую временную шкалу, используя сводную таблицу в качестве данных source
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* пространство имен [Aspose.Cells.Timelines](../../timelinecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Имя ячейки в верхнем левом углу диапазона временной шкалы. |
| baseFieldIndex | Int32 | Индекс PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый добавленный индекс временной шкалы

### Примеры

```csharp

[C#]
  //Добавить новую временную шкалу, используя сводную таблицу в качестве данных source
sheet.Timelines.Add(pivot, "i5", 1);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* пространство имен [Aspose.Cells.Timelines](../../timelinecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона временной шкалы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона временной шкалы. |
| baseField | PivotField | PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс временной шкалы

### Примеры

```csharp

[C#]
  //Добавить новую временную шкалу, используя сводную таблицу в качестве данных source
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* пространство имен [Aspose.Cells.Timelines](../../timelinecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Имя ячейки в верхнем левом углу диапазона временной шкалы. |
| baseField | PivotField | PivotField в PivotTable.BaseFields |

### Возвращаемое значение

Новый индекс временной шкалы

### Примеры

```csharp

[C#]
  //Добавить новую временную шкалу, используя сводную таблицу в качестве данных source
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### Смотрите также

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* пространство имен [Aspose.Cells.Timelines](../../timelinecollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
