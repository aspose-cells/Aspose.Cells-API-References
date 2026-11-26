---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Скрытый столбец — ширина этого столбца в Excel равна 0. Перед сохранением в формат html, если HtmlHiddenColDisplayType установлен в Remove, скрытый столбец не будет выводиться; если значение — Hidden, столбец будет выводиться, но будет скрыт. Значение по умолчанию — Hidden."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Скрытый столбец (ширина этого столбца 0) в Excel, перед сохранением в html‑формат, если HtmlHiddenColDisplayType равно "Remove", скрытый столбец не будет выводиться, если значение "Hidden", столбец будет выводиться, но будет скрыт, значение по умолчанию — "Hidden".

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Скрыть столбец C (индекс 2)
            worksheet.Cells.HideColumn(2);

            // Добавьте некоторые данные для демонстрации
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // Создать параметры сохранения HTML с различными настройками HiddenColDisplayType
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // Сохранить с различными параметрами
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### См. также

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


