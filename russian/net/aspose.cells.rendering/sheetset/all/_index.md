---
title: "SheetSet.All"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SheetSet. Возвращает набор со всеми листами книги в их исходном порядке"
type: docs
url: /ru/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Получает набор со всеми листами книги в их исходном порядке.

```csharp
public static SheetSet All { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // Создать книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Установите некоторые примерные данные в обоих листах
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Сохраните все листы в markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### См. также

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


