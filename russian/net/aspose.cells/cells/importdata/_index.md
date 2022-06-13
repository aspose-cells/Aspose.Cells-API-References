---
title: ImportData
second_title: Справочник по Aspose.Cells для .NET API
description: Импортирует данные из объектаIDataReader.
type: docs
weight: 970
url: /ru/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Импортирует данные из объектаIDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| reader | IDataReader | ОбъектIDataReader, содержащий данные. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |

### Возвращаемое значение

Общее количество импортированных строк.

### Смотрите также

* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Импортирует данные из объектаIDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| reader | IDataReader | ОбъектIDataReader, содержащий данные. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| options | ImportTableOptions | Параметры импорта таблицы. |

### Возвращаемое значение

Общее количество импортированных строк.

### Смотрите также

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Импорт данных из пользовательской таблицы данных.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| table | ICellsDataTable | Пользовательская таблица данных. |
| firstRow | Int32 | Индекс первой строки. |
| firstColumn | Int32 | Индекс первого столбца. |
| options | ImportTableOptions | Параметры импорта |

### Смотрите также

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Импорт данных из пользовательской таблицы данных.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| table | DataTable | Импортируемый объектDataTable. |
| firstRow | Int32 | Индекс первой строки. |
| firstColumn | Int32 | Индекс первого столбца. |
| options | ImportTableOptions | Параметры импорта |

### Возвращаемое значение

Общее количество импортированных строк.

### Примеры

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

  //Импорт data
DataTable dt = new DataTable("Products");
dt.Columns.Add("Product_ID",typeof(Int32));
dt.Columns.Add("Product_Name",typeof(string));
dt.Columns.Add("Units_In_Stock",typeof(Int32));
DataRow dr = dt.NewRow();
dr[0] = 1;
dr[1] = "Aniseed Syrup";
dr[2] = 15;
dt.Rows.Add(dr);
dr = dt.NewRow();
dr[0] = 2;
dr[1] = "Boston Crab Meat";
dr[2] = 123;
dt.Rows.Add(dr);
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;
cells.ImportData(dt, 12, 12, options);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Import data
Dim dt as DataTable = new DataTable("Employee")
dt.Columns.Add("Employee_ID",typeof(Int32))
dt.Columns.Add("Employee_Name",typeof(string))
dt.Columns.Add("Gender",typeof(string))
Dim dr as DataRow = dt.NewRow()
dr(0) = 1
dr(1) = "John Smith"
dr(2) = "Male"
dt.Rows.Add(dr)
dr = dt.NewRow()
dr(0) = 2
dr(1) = "Mary Miller"
dr(2) = "Female"
dt.Rows.Add(dr)
Dim options as ImportTableOptions = new ImportTableOptions()
options.IsFieldNameShown = True
cells.ImportData(dt, 12, 12, options)

'Export data
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Смотрите также

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Импорт данных из представления данных.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataView | DataView | Импортируемый объектDataView. |
| firstRow | Int32 | Индекс первой строки. |
| firstColumn | Int32 | Индекс первого столбца. |
| options | ImportTableOptions | Параметры импорта |

### Возвращаемое значение

Общее количество импортированных строк.

### Смотрите также

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
