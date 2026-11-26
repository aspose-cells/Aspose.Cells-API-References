---
title: "PptxSaveOptions.AdjustFontSizeForRowType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PptxSaveOptions. Представляет тип строки, для которой необходимо скорректировать размер шрифта, если высота строки небольшая"
type: docs
url: /ru/net/aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/
---
## PptxSaveOptions.AdjustFontSizeForRowType property

Представляет тип линии, для которой необходимо корректировать размер шрифта, если высота строки мала.

```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные и пустые строки
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue(""); // Empty row
            worksheet.Cells["A4"].PutValue("Data 2");
            
            // Создайте параметры сохранения PPTX
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows;
            
            // Сохранить в PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("File saved with AdjustFontSizeForRowType setting");
        }
    }
}
```

### См. также

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


