---
title: "CellsHelper.DPI"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Получает DPI устройства"
type: docs
url: /ru/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Получает DPI машины.

```csharp
public static double DPI { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // Установить и отобразить текущий DPI
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // Изменить настройку DPI
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // Создать новую книгу и сохранить с различными настройками DPI
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить образец фигуры для демонстрации эффекта DPI
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // Сохранить с текущей настройкой DPI
            workbook.Save("output_with_dpi_300.xlsx");

            // Изменить DPI и сохранить снова
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


