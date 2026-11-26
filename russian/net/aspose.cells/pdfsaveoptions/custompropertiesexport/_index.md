---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Получает или задает значение, определяющее способ экспорта CustomDocumentPropertyCollection в PDF‑файл. Значение по умолчанию — None"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

Получает или задает значение, определяющее способ экспорта [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) в PDF‑файл. Значение по умолчанию — None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCustomPropertiesExportDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("Sample PDF Export");

            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Subject", "Aspose.Cells Example");

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            workbook.Save("PdfCustomPropertiesExportDemo.pdf", saveOptions);
        }
    }
}
```

### См. также

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


