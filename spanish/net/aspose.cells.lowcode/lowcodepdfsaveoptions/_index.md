---
title: "Clase LowCodePdfSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodePdfSaveOptions. Opciones para guardar PDF de forma de bajo código"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

Opciones para guardar pdf de forma low code.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Obtiene y establece el archivo (con ruta si es necesario) para guardar los datos generados. Al establecer esta propiedad con un valor distinto de null o cadena vacía, [`OutputStream`](../lowcodesaveoptions/outputstream/) será ignorado.(Hereda de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Obtiene y establece el Stream para escribir los datos generados. Al establecer esta propiedad con un valor distinto de null, [`OutputFile`](../lowcodesaveoptions/outputfile/) será ignorado.(Hereda de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | Las opciones para guardar el archivo PDF. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | El formato de guardado para la salida. Para convertir a PDF, solo puede ser PDF. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // Crear opciones de guardado PDF de bajo código
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // Guardar usando opciones de bajo código
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


