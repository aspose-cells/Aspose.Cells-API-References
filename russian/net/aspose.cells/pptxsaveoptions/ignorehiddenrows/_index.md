---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PptxSaveOptions. Указывает, игнорировать ли скрытые строки при конвертации Excel в PowerPoint"
type: docs
url: /ru/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Указывает, следует ли игнорировать скрытые строки при преобразовании Excel в PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные и скрыть некоторые строки
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Скрыть строку 2
            worksheet.Cells.Rows[1].IsHidden = true;

            // Установить параметры сохранения PPTX с IgnoreHiddenRows
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // Сохранить как PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### См. также

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


