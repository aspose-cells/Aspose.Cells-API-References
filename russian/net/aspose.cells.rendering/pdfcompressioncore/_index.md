---
title: "Перечисление PdfCompressionCore"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Rendering.PdfCompressionCore перечисление. Указывает тип сжатия, применяемый ко всему содержимому PDF‑файла, кроме изображений."
type: docs
url: /ru/net/aspose.cells.rendering/pdfcompressioncore/
---
## PdfCompressionCore enumeration

Указывает тип сжатия, применяемый ко всему содержимому PDF‑файла, кроме изображений.

```csharp
public enum PdfCompressionCore
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет |
| Rle | `1` | Rle |
| Lzw | `2` | Lzw |
| Flate | `3` | Flate |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCompressionCoreDemo
    {
        public static void PdfCompressionCoreExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose!");

            // Создайте PdfSaveOptions и установите PdfCompressionCore
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate

            // Сохраните рабочую книгу в виде PDF‑файла с указанным сжатием
            workbook.Save("PdfCompressionCoreExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file saved with specified compression.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


