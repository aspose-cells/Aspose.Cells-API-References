---
title: "LoadOptions.CultureInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает или задает региональные настройки, используемые для загружаемого Workbook."
type: docs
url: /ru/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Получает или задает региональные настройки, используемые для загружаемой Workbook.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Примечания

Это свойство имеет тот же эффект, что и [`Region`](../region/) для установки региональных настроек.

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Создать пример файла Excel
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // Загрузить с определённой культурой
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


