---
title: "Cells.ExportDataTableAsString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Экспортирует данные из коллекции Cells в объект DataTable"
type: docs
url: /ru/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

Экспортирует данные из коллекции [`Cells`](../) в объект DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для импорта. |
| totalColumns | Int32 | Количество столбцов для импорта. |

### Возвращаемое значение

Экспортированный объект DataTable.

### Примечания

Все данные в коллекции [`Cells`](../) преобразуются в строки.

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавить примерные данные в ячейки
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // Экспортировать данные в DataTable в виде строк
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // Отобразить экспортированные данные
            Console.WriteLine("Exported DataTable:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.Write(column.ColumnName + "\t");
            }
            Console.WriteLine();
            
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item.ToString() + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

Экспортирует данные из коллекции [`Cells`](../) в объект DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для импорта. |
| totalColumns | Int32 | Количество столбцов для импорта. |
| exportColumnName | Boolean | Указывает, экспортируются ли данные первой строки в имена столбцов DataTable. |

### Возвращаемое значение

Экспортированный объект DataTable.

### Примечания

Все данные в коллекции [`Cells`](../) преобразуются в строки.

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Экспортировать данные в DataTable
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // Отобразить экспортированные данные
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (DataColumn col in dataTable.Columns)
                {
                    Console.Write(row[col] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


