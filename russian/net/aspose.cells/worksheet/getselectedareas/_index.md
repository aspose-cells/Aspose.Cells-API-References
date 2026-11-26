---
title: "Worksheet.GetSelectedAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet method. Получает выбранные диапазоны ячеек в конструкторе таблицы"
type: docs
url: /ru/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Получает выбранные диапазоны ячеек в проектируемой таблице.

```csharp
public Range[] GetSelectedAreas()
```

### Возвращаемое значение

Возвращает все выбранные диапазоны.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Выбрать несколько диапазонов
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // Получить выбранные области
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // Показать информацию о выбранных областях
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // Очистить выделения и выбрать один диапазон
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // Получить единственную выбранную область
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


