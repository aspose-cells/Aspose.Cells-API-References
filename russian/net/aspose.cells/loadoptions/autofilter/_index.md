---
title: "LoadOptions.AutoFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Указывает, применяется ли автоматическая фильтрация данных при загрузке файлов"
type: docs
url: /ru/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Указывает, следует ли автоматически фильтровать данные при загрузке файлов.

```csharp
public bool AutoFilter { get; set; }
```

### Примечания

Иногда, несмотря на включенный autofilter, соответствующие строки не скрываются в файле. Сейчас работает только для файлов SpreadSheetML.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки и включите AutoFilter
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // Загрузите книгу с включённым AutoFilter
            Workbook workbook = new Workbook("example.xlsx", options);

            // Получите доступ к первому листу и примените AutoFilter
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


