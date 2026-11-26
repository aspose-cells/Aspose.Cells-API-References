---
title: "Перечисление PdfCustomPropertiesExport"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.PdfCustomPropertiesExport. Указывает способ экспорта CustomDocumentPropertyCollection в PDF‑файл"
type: docs
url: /ru/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

Указывает способ экспорта [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) в PDF‑файл.

```csharp
public enum PdfCustomPropertiesExport
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Пользовательские свойства не экспортируются. |
| Standard | `1` | Пользовательские свойства экспортируются как записи в словаре Info. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCustomPropertiesExportDemo
    {
        public static void PdfCustomPropertiesExportExample()
        {
            // Создайте книгу и добавьте некоторые данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // Установите некоторые пользовательские свойства
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // Создайте параметры сохранения PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Установите параметр экспорта пользовательских свойств
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // Сохраните книгу в PDF
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


