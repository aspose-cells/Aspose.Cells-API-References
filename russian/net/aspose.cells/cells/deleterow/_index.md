---
title: "Cells.DeleteRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет строку"
type: docs
url: /ru/net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

Удаляет строку.

```csharp
public void DeleteRow(int rowIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки, которую нужно удалить. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Установите общую формулу в строке 66
            cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);

            // Удалите строку 9 (это сдвинет строки вверх)
            cells.DeleteRow(9);

            // Проверьте, что формула была скорректирована после удаления строки
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
            }

            // Удалите строки 60‑61 (это сдвинет строки вверх)
            cells.DeleteRows(59, 2);

            // Проверьте, что формула была скорректирована после удаления строк
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
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

## DeleteRow(int, bool) {#deleterow_1}

Удаляет строку.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки, которую нужно удалить. |
| updateReference | Boolean | Указывает, следует ли обновлять ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            sheet.Cells.DeleteRow(2, true);

            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            workbook.Save("DeleteRowExample.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


