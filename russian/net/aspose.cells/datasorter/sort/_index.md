---
title: Sort
second_title: Справочник по Aspose.Cells для .NET API
description: Сортирует данные области.
type: docs
weight: 140
url: /ru/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Сортирует данные области.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cells | Cells | Ячейки содержат область данных. |
| startRow | Int32 | Стартовый ряд площади. |
| startColumn | Int32 | Начальный столбец области. |
| endRow | Int32 | Крайний ряд площади. |
| endColumn | Int32 | Конечная колонка области. |

### Возвращаемое значение

исходные индексы (абсолютная позиция, например, столбец A равен 0, B равен 1, ...) отсортированных строк/столбцов. Если при этой операции сортировки не требуется перемещать строки/столбцы, будет возвращено значение null.

### Смотрите также

* class [Cells](../../cells)
* class [DataSorter](../../datasorter)
* пространство имен [Aspose.Cells](../../datasorter)
* сборка [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Сортировка данных области.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cells | Cells | Ячейки содержат область данных. |
| area | CellArea | Площадь, необходимая для сортировки |

### Возвращаемое значение

исходные индексы (абсолютная позиция, например, столбец A равен 0, B равен 1, ...) отсортированных строк/столбцов. Если при этой операции сортировки не требуется перемещать строки/столбцы, будет возвращено значение null.

### Смотрите также

* class [Cells](../../cells)
* struct [CellArea](../../cellarea)
* class [DataSorter](../../datasorter)
* пространство имен [Aspose.Cells](../../datasorter)
* сборка [Aspose.Cells](../../../)

---

## Sort() {#sort}

Сортировать данные в диапазоне.

```csharp
public int[] Sort()
```

### Возвращаемое значение

исходные индексы (абсолютная позиция, например, столбец A равен 0, B равен 1, ...) отсортированных строк/столбцов. Если при этой операции сортировки не требуется перемещать строки/столбцы, будет возвращено значение null.

### Смотрите также

* class [DataSorter](../../datasorter)
* пространство имен [Aspose.Cells](../../datasorter)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
