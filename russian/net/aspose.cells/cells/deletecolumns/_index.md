---
title: "Cells.DeleteColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет несколько столбцов"
type: docs
url: /ru/net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Удаляет несколько столбцов.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс первого столбца для удаления. |
| totalColumns | Int32 | Количество столбцов для удаления. |
| updateReference | Boolean | Указывает, следует ли обновлять ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Добавить формулу, ссылающуюся на эти столбцы
            worksheet.Cells["D1"].Formula = "=SUM(A2:C2)";

            Console.WriteLine("Before deleting columns:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1: " + worksheet.Cells["C1"].Value);
            Console.WriteLine("D1 formula: " + worksheet.Cells["D1"].Formula);

            // Удалить столбец B (индекс 1) и сдвинуть оставшиеся столбцы влево
            worksheet.Cells.DeleteColumns(1, 1, true);

            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1 formula: " + worksheet.Cells["C1"].Formula);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Удаляет несколько столбцов.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс первого столбца для удаления. |
| totalColumns | Int32 | Количество столбцов для удаления. |
| опции | DeleteOptions | Параметры операции удаления |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить примерными данными столбцы A‑E
            for (int col = 0; col < 5; col++)
            {
                worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
                worksheet.Cells[1, col].Value = $"Data{col + 1}";
            }

            // Создать DeleteOptions и настроить параметры
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Update references in other cells
            };

            try
            {
                // Удалить 2 столбца, начиная со столбца B (индекс 1)
                worksheet.Cells.DeleteColumns(1, 2, options);
                
                Console.WriteLine("Deleted columns B and C successfully");
                
                // Отобразить оставшиеся данные в столбце B (исходный столбец D)
                Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
            }
            
            // Сохранить изменённую книгу
            workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


