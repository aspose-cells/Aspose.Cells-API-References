---
title: "Cells.DeleteBlankColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет все пустые столбцы, которые не содержат данных"
type: docs
url: /ru/net/aspose.cells/cells/deleteblankcolumns/
---
## DeleteBlankColumns() {#deleteblankcolumns}

Удаляет все пустые столбцы, которые не содержат никаких данных.

```csharp
public void DeleteBlankColumns()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые тестовые данные с пустыми столбцами
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B will be blank
            worksheet.Cells["A2"].PutValue("Data A");
            worksheet.Cells["C2"].PutValue("Data C");
            
            // Удалить пустые столбцы
            worksheet.Cells.DeleteBlankColumns();
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankColumns(DeleteOptions) {#deleteblankcolumns_1}

Удаляет все пустые столбцы, которые не содержат никаких данных.

```csharp
public void DeleteBlankColumns(DeleteOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | DeleteOptions | Параметры удаления диапазона. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные с пустыми столбцами
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B is blank
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["C2"].PutValue(3);

            Console.WriteLine("Before deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 2 (0-based, column C)

            // Настройте параметры удаления
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;

            // Удалить пустые столбцы
            worksheet.Cells.DeleteBlankColumns(options);

            Console.WriteLine("After deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 1 (0-based, column A and C remain, B was deleted)

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


