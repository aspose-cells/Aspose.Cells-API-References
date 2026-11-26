---
title: "HtmlSaveOptions.CssStyles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает или задаёт дополнительные CSS‑стили для форматировщика. Работает только когда SaveAsSingleFile равно True.  CssStylesbody  padding 5px"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

Получает или задаёт дополнительные CSS‑стили для форматировщика. Работает только когда [`SaveAsSingleFile`](../saveassinglefile/) равно True.  CssStyles="body { padding: 5px }";

```csharp
public string CssStyles { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCssStylesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установите пользовательские CSS‑стили
            saveOptions.CssStyles = @"
                body { 
                    font-family: Arial;
                    background-color: #f0f0f0;
                }
                table {
                    border-collapse: collapse;
                    width: 100%;
                }
                td {
                    border: 1px solid #ddd;
                    padding: 8px;
                }";

            // Сохраните книгу с пользовательскими CSS‑стилями
            workbook.Save("HtmlWithCustomStyles.html", saveOptions);

            Console.WriteLine("HTML file with custom CSS styles created successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


