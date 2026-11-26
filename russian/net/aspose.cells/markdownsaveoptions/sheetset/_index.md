---
title: "MarkdownSaveOptions.SheetSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге Active"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/sheetset/
---
## MarkdownSaveOptions.SheetSet property

Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Active`](../../../aspose.cells.rendering/sheetset/active/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Примечания

Набор игнорируется, когда он используется в [`SheetRender`](../../../aspose.cells.rendering/sheetrender/)

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("Sheet1 Data");
            
            // Добавить второй лист
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Data");

            // Создайте параметры сохранения Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Сохраните все листы в markdown
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save("output_all_sheets.md", saveOptions);
            
            // Сохраните только первый лист
            saveOptions.SheetSet = new SheetSet(new int[] { 0 });
            workbook.Save("output_first_sheet.md", saveOptions);
        }
    }
}
```

### См. также

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


