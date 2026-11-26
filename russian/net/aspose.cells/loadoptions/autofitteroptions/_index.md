---
title: "LoadOptions.AutoFitterOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает и задаёт параметры автоподгонки"
type: docs
url: /ru/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Получает и задает параметры автоподгонки

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Примечания

Только для файлов xlsx, spreadsheetML сейчас.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Создать AutoFitterOptions и задать свойства
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // Создать LoadOptions и назначить AutoFitterOptions
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // Загрузить рабочую книгу с указанными параметрами
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // Продемонстрировать автоподгонку, получив высоту строки
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


