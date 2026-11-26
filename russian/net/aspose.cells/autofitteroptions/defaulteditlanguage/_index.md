---
title: "AutoFitterOptions.DefaultEditLanguage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Получает или задает язык редактирования по умолчанию"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Получает или задает язык редактирования по умолчанию.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Примечания

Он может отображать/рендерить разные макеты абзаца текста при установленном различном языке редактирования. По умолчанию — Auto.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите пример текста CJK в ячейку
            worksheet.Cells["A1"].PutValue("日本語のテキスト");

            AutoFitterOptions options = new AutoFitterOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Автоподгонка строки с настройками языка CJK
            worksheet.AutoFitRows(options);

            Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
            workbook.Save("DefaultEditLanguageDemo.xlsx");
        }
    }
}
```

### См. также

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


