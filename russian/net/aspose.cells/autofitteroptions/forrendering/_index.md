---
title: "AutoFitterOptions.ForRendering"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Указывает, применяется ли подгонка для целей рендеринга"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Указывает, следует ли подгонка для целей рендеринга.

```csharp
public bool ForRendering { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить образцовые данные с длинным текстом
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // Создать AutoFitterOptions и установить ForRendering в true
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // Автоподогнать строку с учётом рендеринга
            worksheet.AutoFitRows(0, 0, options);

            // Вывести полученную высоту строки в пикселях
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


