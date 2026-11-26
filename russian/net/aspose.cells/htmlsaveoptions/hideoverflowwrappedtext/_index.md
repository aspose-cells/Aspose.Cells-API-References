---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Указывает, следует ли скрывать переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите пример текста в ячейку A1
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // Создайте и примените стиль с переносом текста
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Получите коллекцию ячеек и примените стиль
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // Установите ширину столбца, чтобы текст переносился
            cells.SetColumnWidth(0, 10);
            
            // Создайте параметры сохранения HTML и установите HideOverflowWrappedText
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // Сохранить книгу с параметрами HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


