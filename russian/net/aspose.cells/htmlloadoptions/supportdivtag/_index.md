---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Указывает, поддерживается ли разметка тега div, когда HTML‑файл содержит его. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Указывает, поддерживается ли макет тега `<div>`, когда HTML‑файл содержит его. Значение по умолчанию — false.

```csharp
public bool SupportDivTag { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML с включённым SupportDivTag
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // Загрузить HTML‑файл с тегами div
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // Получить доступ к данным первого листа
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Вывести значение ячейки и информацию о стиле
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // Сохранить как файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


