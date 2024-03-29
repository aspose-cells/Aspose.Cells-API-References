---
title: ExportDataTable
second_title: Справочник по Aspose.Cells для .NET API
description: Экспортирует данные вCellsaspose.cells/cells сбор вDataTable объект.
type: docs
weight: 610
url: /ru/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

Экспортирует данные в[`Cells`](../../cells) сбор вDataTable объект.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для импорта. |
| totalColumns | Int32 | Количество столбцов, которые необходимо импортировать. |

### Возвращаемое значение

ЭкспортированоDataTable объект.

### Примечания

Если вы используете этот метод для экспорта блока данных, убедитесь, что данные в столбце должны быть одного типа. В противном случае используйте[`ExportDataTableAsString`](../exportdatatableasstring)метод вместо этого.

### Примеры

```csharp
[C#]


string designerFile = "List.xls";
Workbook excel = new Workbook(designerFile);
Worksheet sheet = excel.Worksheets[0];
DataTable dt = sheet.Cells.ExportDataTable(6, 1, 69, 4);

[Visual Basic]


Dim designerFile As String = "List.xls"
Dim excel As excel = New excel(designerFile)
Dim sheet As Worksheet = excel.Worksheets(0)
Dim dt As DataTable = sheet.Cells.ExportDataTable(6, 1, 69, 4)
```

### Смотрите также

* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

Экспортирует данные в[`Cells`](../../cells) сбор вDataTable объект.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для импорта. |
| totalColumns | Int32 | Количество столбцов, которые необходимо импортировать. |
| exportColumnName | Boolean | Указывает, экспортируются ли данные в первой строке в имя столбца DataTable. |

### Возвращаемое значение

ЭкспортированоDataTable объект.

### Смотрите также

* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

Экспортирует данные в[`Cells`](../../cells) сбор вDataTable объект.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для импорта. |
| totalColumns | Int32 | Количество столбцов, которые необходимо импортировать. |
| options | ExportTableOptions | Все параметры таблицы экспорта |

### Возвращаемое значение

ЭкспортированоDataTable объект.

### Смотрите также

* class [ExportTableOptions](../../exporttableoptions)
* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
