---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Indica si se exporta la estructura del documento"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Indica si se debe exportar la estructura del documento.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Establezca ExportDocumentStructure a true para conservar la estructura del documento
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // Calcule las fórmulas antes de guardar
            workbook.CalculateFormula();

            // Guardar el libro de trabajo en PDF con las opciones especificadas
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


