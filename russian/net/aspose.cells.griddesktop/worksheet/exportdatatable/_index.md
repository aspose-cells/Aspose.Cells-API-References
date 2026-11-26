---
title: "Worksheet.ExportDataTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Экспортирует данные из коллекции Cells листа в указанный объект DataTable."
type: docs
url: /ru/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

Экспортирует данные из коллекции Cells листа Worksheet в указанный объект DataTable.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для экспорта. |
| startColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| isVertical | Boolean | True, если строка в элементе управления представляет строку в DataTable. False, если столбец в элементе управления представляет строку в DataTable. |

### Возвращаемое значение

Экспортированный объект DataTable.

### Примечания

Метод позволяет сначала создать объект DataTable. Затем экспортирует данные в объект DataTable. Если dataTable не установлен корректно, метод вернёт новый объект DataTable, вызвав перегруженный метод 'Export(bool exportColumnName, bool isVertical)'.

### Примеры

```csharp
[C#]

DataTable dataTable = new DataTable();
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"));
dataTable.Columns.Add("Column b");
dataTable.Columns.Add("Column c");
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"));
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"));
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"));
DataTable exportTable = gridDesktop.Worksheets[0].Export(dataTable,1,0,10,6,true);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim dataTable As DataTable =  New DataTable() 
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"))
dataTable.Columns.Add("Column b")
dataTable.Columns.Add("Column c")
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"))
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"))
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"))
Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(dataTable,1,0,10,6,True) 
DataGrid1.SetDataBinding(exportTable)
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

Экспортирует данные из коллекции Cells листа Worksheet в новый объект DataTable.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для экспорта. |
| startColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| exportColumnName | Boolean | Указывает, экспортируются ли данные первой строки в имена столбцов DataTable. |
| isVertical | Boolean | True, если строка в элементе управления представляет строку в DataTable. False, если столбец в элементе управления представляет строку в DataTable. |

### Возвращаемое значение

Экспортированный объект DataTable.

### Примеры

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

Экспортирует данные из коллекции [`Cells`](../cells/) в объект DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для импорта. |
| totalColumns | Int32 | Количество столбцов для импорта. |
| опции | GridExportTableOptions | Все параметры экспорта таблицы |

### Возвращаемое значение

Экспортированный объект DataTable.

### См. также

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


