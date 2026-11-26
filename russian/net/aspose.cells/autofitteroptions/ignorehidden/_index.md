---
title: "AutoFitterOptions.IgnoreHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Игнорирует скрытые строки/столбцы"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Игнорирует скрытые строки/столбцы.

```csharp
public bool IgnoreHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyIgnoreHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерные данные и отформатировать строки
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["A2"].PutValue("Another test string");
            
            // Скрыть строку 1
            worksheet.Cells.Rows[1].IsHidden = true;

            // Создать AutoFitterOptions с параметром IgnoreHidden, установленным в true
            AutoFitterOptions options = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCells = false,
                OnlyAuto = false
            };

            // Автоподгонка строк при игнорировании скрытых строк
            worksheet.AutoFitRows(options);

            // Вывести высоты строк
            Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
            Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


