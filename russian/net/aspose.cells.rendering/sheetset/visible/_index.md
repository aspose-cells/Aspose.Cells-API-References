---
title: "SheetSet.Visible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SheetSet. Возвращает набор с видимыми листами книги в их исходном порядке"
type: docs
url: /ru/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Получает набор с видимыми листами книги в их исходном порядке.

```csharp
public static SheetSet Visible { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Скрыть второй лист
            workbook.Worksheets[1].IsVisible = false;

            // Настройте параметры сохранения, чтобы экспортировать только видимые листы
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // Сохраните книгу (будет экспортирован только видимый лист)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### См. также

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


