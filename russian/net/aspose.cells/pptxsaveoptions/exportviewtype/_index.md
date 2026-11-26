---
title: "PptxSaveOptions.ExportViewType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PptxSaveOptions. Получает и задает тип отображения при экспорте в PowerPoint. Тип экспорта по умолчанию работает как печать"
type: docs
url: /ru/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

Получает и задает тип отображения при экспорте в PowerPoint. Тип экспорта по умолчанию работает как печать.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyExportViewTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Установить параметры сохранения PPTX с ExportViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // Сохранить книгу в формате PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### См. также

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


