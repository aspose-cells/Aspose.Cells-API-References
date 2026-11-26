---
title: "LoadOptions.Region"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает или задает региональные настройки, используемые для загружаемого Workbook."
type: docs
url: /ru/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Получает или задает региональные настройки, используемые для загружаемой Workbook.

```csharp
public CountryCode Region { get; set; }
```

### Примечания

Региональные настройки могут использоваться для инициализации некоторых функций книги, таких как шрифты, темы и т.д. Для текстовых форматов файлов, таких как CSV, HTML, ..., региональная настройка также будет использоваться для определения форматов чисел и преобразования текстовых значений в числовые или datetime‑значения ячеек. Эта настройка будет сохранена для созданной позже книги, то есть [`Region`](../../workbooksettings/region/) книги будет использовать тот же регион, что и это свойство.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки для HTML‑файла
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Установите регион в USA
            loadOpts.Region = CountryCode.USA;
            
            // Загрузите HTML‑файл с указанными региональными настройками
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // Получить доступ к первому листу
            Worksheet ws = wb.Worksheets[0];
            
            // Продемонстрируйте региональное форматирование, проверив стиль ячейки
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### См. также

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


