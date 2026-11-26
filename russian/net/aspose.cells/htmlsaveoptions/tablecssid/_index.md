---
title: "HtmlSaveOptions.TableCssId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает и задает префикс имени типа CSS, например trcoltd и т.д., которые находятся в элементе table, имеющем атрибут TableCssId. Значение по умолчанию — "
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

Получает и задает префикс имени типа css, например tr, col, td и т.д., они находятся в элементе table, который имеет атрибут TableCssId. Значение по умолчанию — "".

```csharp
public string TableCssId { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyTableCssIdDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Настройте параметры сохранения HTML с TableCssId
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.TableCssId = "custom-table-style";
            
            // Сохранить рабочую книгу с параметрами HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with TableCssId: " + saveOptions.TableCssId);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


