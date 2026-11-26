---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptions. Obtiene y establece el archivo con ruta si es necesario para guardar los datos generados. Al establecer esta propiedad con un valor distinto de null o cadena vacía, OutputStream será ignorado."
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Obtiene y establece el archivo (con ruta si es necesario) para guardar los datos generados. Al establecer esta propiedad con un valor distinto de null o cadena vacía, [`OutputStream`](../outputstream/) será ignorado.

```csharp
public string OutputFile { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeSaveOptionsPropertyOutputFileDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo sencillo con una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Guardar en diferentes formatos usando la propiedad OutputFile
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Guardar como PDF
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // Guardar como JSON
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // Guardar como HTML
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // Guardar como CSV
            SaveWithOutputFile(workbook, SaveFormat.Csv, "output.csv");
        }

        private static void SaveWithOutputFile(Workbook workbook, SaveFormat format, string fileName)
        {
            string outputPath = "Output/" + fileName;
            
            switch (format)
            {
                case SaveFormat.Pdf:
                    PdfConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodePdfSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Json:
                    JsonConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Html:
                    HtmlConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Csv:
                    TextConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                default:
                    throw new NotSupportedException("Format not supported: " + format);
            }

            Console.WriteLine($"File saved successfully to: {outputPath}");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


