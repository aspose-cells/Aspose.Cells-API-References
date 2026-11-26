---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PasteOptions. Игнорировать ссылки на оригинальный файл"
type: docs
url: /ru/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Игнорировать ссылки на оригинальный файл.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // Создать примерные данные с формулами, которые могут ссылаться на оригинальный файл
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // Создать целевой рабочий лист и диапазон
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // Настроить параметры вставки, чтобы игнорировать ссылки на оригинальный файл
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // Копировать с указанными параметрами вставки
            dstRange.Copy(srcRange, pasteOptions);

            // Сохраните книгу
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### См. также

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


