---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Скрытая строка: высота этой строки в Excel равна 0. Перед сохранением в формат HTML, если HtmlHiddenRowDisplayType установлен в Remove, скрытая строка не будет выводиться; если значение — Hidden, строка будет выводиться, но будет скрытой. Значение по умолчанию — Hidden."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Скрытая строка (высота этой строки 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться, если значение "Hidden", строка будет выводиться, но будет скрыта, значение по умолчанию — "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные и скройте строку.
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // Установите параметры сохранения HTML с HiddenRowDisplayType.
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // Сохранить в HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### См. также

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


