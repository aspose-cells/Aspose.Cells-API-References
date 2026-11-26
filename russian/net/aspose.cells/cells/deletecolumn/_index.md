---
title: "Cells.DeleteColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет столбец"
type: docs
url: /ru/net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Удаляет столбец.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца, который будет удалён. |
| updateReference | Boolean | Указывает, следует ли обновлять ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Заполните некоторые примерные данные в ячейки
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }
            
            Console.WriteLine("Before deleting column:");
            PrintCellValues(sheet);
            
            // Удалите первый столбец и сдвиньте оставшиеся столбцы влево
            sheet.Cells.DeleteColumn(0, true);
            
            Console.WriteLine("\nAfter deleting column 0:");
            PrintCellValues(sheet);
            
            // Сохраните книгу
            workbook.Save("DeleteColumnDemo.xlsx");
        }
        
        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    Console.Write(sheet.Cells[i, j].Value + "\t");
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

## DeleteColumn(int) {#deletecolumn}

Удаляет столбец.

```csharp
public void DeleteColumn(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца, который будет удалён. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Заполните некоторые примерные данные в столбцах
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Удалить столбец с индексом 1 (Столбец B)
            cells.DeleteColumn(1);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Column deleted successfully.");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


