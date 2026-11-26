---
title: "Перечисление PdfCompliance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.PdfCompliance. Позволяет пользователю задавать совместимость при конвертации в PDF"
type: docs
url: /ru/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

Позволяет пользователю установить совместимость конвертации PDF.

```csharp
public enum PdfCompliance
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Формат PDF, совместимый с PDF 1.4 |
| Pdf14 | `0` | Формат PDF, совместимый с PDF 1.4 |
| Pdf15 | `3` | Формат PDF, совместимый с PDF 1.5 |
| Pdf16 | `4` | Формат PDF, совместимый с PDF 1.6 |
| Pdf17 | `5` | Формат PDF, совместимый с PDF 1.7 |
| PdfA1b | `1` | Формат PDF, совместимый с PDF/A-1b (ISO 19005-1) |
| PdfA1a | `2` | Формат PDF, совместимый с PDF/A-1a (ISO 19005-1) |
| PdfA2b | `6` | Формат PDF, совместимый с PDF/A-2b (ISO 19005-2) |
| PdfA2u | `7` | Формат PDF, совместимый с PDF/A-2u (ISO 19005-2) |
| PdfA2a | `8` | Формат PDF, совместимый с PDF/A-2a (ISO 19005-2) |
| PdfA3b | `9` | Формат PDF, совместимый с PDF/A-3b(ISO 19005-3) |
| PdfA3u | `10` | Формат PDF, совместимый с PDF/A-3u(ISO 19005-3) |
| PdfA3a | `11` | Формат PDF, совместимый с PDF/A-3a(ISO 19005-3) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfComplianceDemo
    {
        public static void PdfComplianceExample()
        {
            // Создание рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // Настройка параметров сохранения PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Установка уровня соответствия PDF/A-1b
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // Сохранение рабочей книги в PDF с указанным уровнем соответствия
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


