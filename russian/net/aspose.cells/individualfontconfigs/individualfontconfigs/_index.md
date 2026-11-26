---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор IndividualFontConfigs. Ctor"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

Конструктор.

```csharp
public IndividualFontConfigs()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки с IndividualFontConfigs
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // Создать новую книгу с листом по умолчанию
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // Получить доступ к листу и добавить некоторый текст
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // Сохранить книгу (параметры загрузки не требуются для сохранения)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### См. также

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


