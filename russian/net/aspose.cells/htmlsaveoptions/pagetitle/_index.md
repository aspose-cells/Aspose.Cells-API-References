---
title: "HtmlSaveOptions.PageTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Заголовок html‑страницы. Только при сохранении в html‑поток"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/pagetitle/
---
## HtmlSaveOptions.PageTitle property

Заголовок HTML‑страницы. Только при сохранении в поток HTML.

```csharp
public string PageTitle { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPageTitleDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            // Установите параметры сохранения HTML с PageTitle
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.PageTitle = "My Custom Page Title";

            // Сохранить в HTML с указанным заголовком
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with custom page title: " + outputPath);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


