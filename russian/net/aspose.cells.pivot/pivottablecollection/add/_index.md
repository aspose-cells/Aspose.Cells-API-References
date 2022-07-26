---
title: Add
second_title: Справочник по Aspose.Cells для .NET API
description: Добавляет новый кэш сводной таблицы в коллекцию PivotCaches.
type: docs
weight: 20
url: /ru/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_4}

Добавляет новый кэш сводной таблицы в коллекцию PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Данные для нового кэша сводной таблицы. |
| destCellName | String | Ячейка в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| tableName | String | Имя нового отчета сводной таблицы. |

### Возвращаемое значение

Новый добавленный кеш-индекс.

### Смотрите также

* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_5}

Добавляет новый кэш сводной таблицы в коллекцию PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Данные для нового кэша сводной таблицы. |
| destCellName | String | Ячейка в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| tableName | String | Имя нового отчета сводной таблицы. |
| useSameSource | Boolean | Указывает, используется ли тот же источник данных, когда другая существующая сводная таблица использовала этот источник данных. Если свойство имеет значение true, оно будет экономить память. |

### Возвращаемое значение

Новый добавленный кеш-индекс.

### Смотрите также

* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

Добавляет новый кэш сводной таблицы в коллекцию PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8. |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| tableName | String | Имя нового отчета сводной таблицы. |

### Возвращаемое значение

Новый добавленный кеш-индекс.

### Смотрите также

* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

Добавляет новый кэш сводной таблицы в коллекцию PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8. |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| tableName | String | Имя нового отчета сводной таблицы. |
| useSameSource | Boolean | Указывает, используется ли тот же источник данных, когда другая существующая сводная таблица использовала этот источник данных. Если свойство имеет значение true, оно будет экономить память. |

### Возвращаемое значение

Новый добавленный кеш-индекс.

### Смотрите также

* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

Добавляет новый объект сводной таблицы в коллекцию из другой сводной таблицы.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | PivotTable | Исходная сводная таблица. |
| destCellName | String | Ячейка в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| tableName | String | Имя нового отчета сводной таблицы. |

### Возвращаемое значение

Новый добавленный индекс сводной таблицы.

### Смотрите также

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

Добавляет новый объект сводной таблицы в коллекцию из другой сводной таблицы.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | PivotTable | Исходная сводная таблица. |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| tableName | String | Имя нового отчета сводной таблицы. |

### Возвращаемое значение

Новый добавленный индекс сводной таблицы.

### Смотрите также

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_7}

Добавляет новый объект сводной таблицы в коллекцию с несколькими диапазонами консолидации в качестве источника данных.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String[] | Несколько диапазонов консолидации, например {"Лист1!A1:C8","Лист2!A1:B8"} |
| isAutoPage | Boolean | Будет ли автоматически создаваться одно поле страницы. Если true, следующие параметры pageFields будут игнорироваться. |
| pageFields | PivotPageFields | Элементы поля сводной страницы. |
| destCellName | String | destCellName Имя нового отчета сводной таблицы. |
| tableName | String | имя нового отчета сводной таблицы. |

### Возвращаемое значение

Новый добавленный индекс сводной таблицы.

### Смотрите также

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_6}

Добавляет новый объект сводной таблицы в коллекцию с несколькими диапазонами консолидации в качестве источника данных.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | String[] | Несколько диапазонов консолидации, например {"Лист1!A1:C8","Лист2!A1:B8"} |
| isAutoPage | Boolean | Будет ли автоматически создаваться одно поле страницы. Если true, следующие параметры pageFields будут игнорироваться. |
| pageFields | PivotPageFields | Элементы поля сводной страницы. |
| row | Int32 | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| column | Int32 | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы. |
| tableName | String | Имя нового отчета сводной таблицы. |

### Возвращаемое значение

Новый добавленный индекс сводной таблицы.

### Смотрите также

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* пространство имен [Aspose.Cells.Pivot](../../pivottablecollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
