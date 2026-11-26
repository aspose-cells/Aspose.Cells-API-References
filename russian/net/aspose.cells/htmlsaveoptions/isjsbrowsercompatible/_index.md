---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "HtmlSaveOptions property. Указывает, совместим ли JavaScript с браузерами, которые не поддерживают JavaScript. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. Значение по умолчанию — true.

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // Настройте параметры сохранения HTML с IsJsBrowserCompatible, установленным в true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // Сохраните рабочую книгу с совместимостью JavaScript
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


