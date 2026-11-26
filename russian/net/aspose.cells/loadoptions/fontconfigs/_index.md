---
title: "LoadOptions.FontConfigs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает и задает отдельные конфигурации шрифтов. Работает только для Workbook, который использует эти LoadOptions для загрузки"
type: docs
url: /ru/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

Получает и задает отдельные конфигурации шрифтов. Работает только для [`Workbook`](../../workbook/), который использует эти [`LoadOptions`](../) для загрузки.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyFontConfigsDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки с FontConfigs
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // Установите некоторые правила замены шрифтов, используя правильный API
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // Загрузите CSV‑файл с указанными параметрами
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // Сохраните Workbook в файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


