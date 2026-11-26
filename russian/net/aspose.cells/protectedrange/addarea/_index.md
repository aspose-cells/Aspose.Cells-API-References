---
title: "ProtectedRange.AddArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ProtectedRange. Добавляет ссылочную область к этому"
type: docs
url: /ru/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

Добавляет ссылочную область к этому

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка. |
| startColumn | Int32 | Начальный столбец. |
| endRow | Int32 | Конечная строка. |
| endColumn | Int32 | Конечный столбец. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectedRangeMethodAddAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add возвращает индекс нового ProtectedRange в коллекции
            int protectedRangeIndex = worksheet.AllowEditRanges.Add("DemoProtectedRange", 0, 0, 0, 0);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[protectedRangeIndex];

            try
            {
                protectedRange.AddArea(2, 2, 5, 5);
                Console.WriteLine("Added new area to protected range.");

                CellArea[] areas = protectedRange.GetAreas();
                Console.WriteLine($"Total protected areas: {areas.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            worksheet.Protect(ProtectionType.All, "password123", null);
            workbook.Save("ProtectedRangeAddAreaDemo.xlsx");
        }
    }
}
```

### См. также

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


