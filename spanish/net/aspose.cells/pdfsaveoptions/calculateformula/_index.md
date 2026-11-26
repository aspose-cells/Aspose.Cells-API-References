---
title: "PdfSaveOptions.CalculateFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Indica si se deben calcular las fórmulas antes de guardar el archivo pdf"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

Indica si se deben calcular las fórmulas antes de guardar el archivo pdf.

```csharp
public bool CalculateFormula { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de muestra y fórmulas
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer valores y fórmulas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Crear opciones de guardado PDF con cálculo de fórmulas
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            // Guardar en flujo de memoria
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Restablecer la posición del flujo y verificar el contenido
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine("PDF contains formula results: " + content.Contains("30"));
                }
            }
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


