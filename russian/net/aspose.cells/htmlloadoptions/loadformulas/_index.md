---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Указывает, импортировать ли формулы, если исходный HTML‑файл содержит формулы"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

Указывает, следует ли импортировать формулы, если исходный HTML‑файл содержит формулы

```csharp
public bool LoadFormulas { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // Создать экземпляр HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Установите LoadFormulas в true, чтобы загрузить формулы из HTML
            loadOptions.LoadFormulas = true;

            // Загрузить HTML‑файл, содержащий формулы, в Workbook
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Отобразить формулу из ячейки A1 (если она присутствует в HTML)
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

            // Сохраните Workbook в файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


