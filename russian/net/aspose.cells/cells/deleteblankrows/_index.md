---
title: "Cells.DeleteBlankRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет все пустые строки, которые не содержат данных или других объектов"
type: docs
url: /ru/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Удаляет все пустые строки, которые не содержат никаких данных или других объектов.

```csharp
public void DeleteBlankRows()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавить некоторые данные с пустыми строками
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Удалить пустые строки
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

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

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Удаляет все пустые строки, которые не содержат никаких данных или некоторых специальных объектов, таких как видимый комментарий, сводная таблица.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | DeleteOptions | Параметры удаления диапазона. |

### Примечания

Для пустых строк, которые будут удалены, необходимо не только чтобы [`IsBlank`](../../row/isblank/) было истинным, но также не должно быть видимых комментариев, определённых для любой ячейки в этих строках, и не должно быть сводных таблиц, диапазон которых пересекается с ними.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить тестовые данные с пустыми строками
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // Создать параметры удаления
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // Удалить пустые строки
            sheet.Cells.DeleteBlankRows(options);
            
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


