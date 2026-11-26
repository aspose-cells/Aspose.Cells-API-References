---
title: "LoadOptions.LanguageCode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает или задает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл."
type: docs
url: /ru/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Получает или задает язык пользовательского интерфейса версии Workbook, основанный на CountryCode, который сохранил файл.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Создайте экземпляр LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Установите свойство LanguageCode
            loadOptions.LanguageCode = CountryCode.USA;

            // Загрузите книгу с указанными LoadOptions
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Получите доступ к листу и измените содержимое
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // Сохранить изменённую книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


