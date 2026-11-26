---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptions. Obtiene y establece el formato de guardado para la salida. Generalmente, para procesos específicos en modo low‑code solo se permiten algunos formatos concretos. Por favor, especifique el formato correcto para el proceso correspondiente; de lo contrario, pueden producirse resultados inesperados o incluso excepciones."
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

Obtiene y establece el formato de guardado para la salida. Generalmente, para procesos específicos en modo de bajo código, solo se permiten algunos formatos específicos. Por favor, especifique el formato correcto para el proceso correspondiente, de lo contrario pueden producirse resultados inesperados o incluso excepciones.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Inicializar LowCodeSaveOptions con diferentes formatos
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // Configurar las opciones de guardado de Excel
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // Configurar opciones de guardado de PDF
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // Demostrar el guardado en el formato original
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // Demostrar el cambio de formato y volver a guardar
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


