---
title: "HtmlConverter.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método HtmlConverter. Convierte el archivo de plantilla proporcionado entre html y otros formatos"
type: docs
url: /es/net/aspose.cells.lowcode/htmlconverter/process/
---
## Process(string, string) {#process_1}

Convierte el archivo de plantilla dado entre html y otros formatos.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | String | El archivo de plantilla a convertir |
| resultFile | String | El archivo resultante |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class HtmlConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Crear archivo HTML temporal para la conversión
            string templateFile = CreateSampleHtmlFile();
            string resultFile = "HtmlConversionResult.xlsx";

            try
            {
                // Procesar los archivos directamente usando HtmlConverter
                HtmlConverter.Process(templateFile, resultFile);

                Console.WriteLine($"Successfully converted '{templateFile}' to '{resultFile}'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Limpia el archivo temporal
                if (File.Exists(templateFile))
                {
                    File.Delete(templateFile);
                }
            }
        }

        private static string CreateSampleHtmlFile()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Conversion");
            
            string tempFile = Path.GetTempFileName() + ".html";
            workbook.Save(tempFile, SaveFormat.Html);
            return tempFile;
        }
    }
}
```

### Ver también

* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convierte archivos entre html y otros formatos de archivo de hoja de cálculo.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones de salida y guardado |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class HtmlConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Crear una plantilla HTML simple en memoria
            string htmlContent = "<html><body><h1>Test Document</h1><p>This is a test HTML document.</p></body></html>";
            using (MemoryStream template = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(htmlContent)))
            {
                // Convertir a PDF usando opciones LowCode
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.pdf",
                        SaveFormat = SaveFormat.Pdf
                    });

                // Restablecer la posición del flujo para la siguiente conversión
                template.Position = 0;

                // Convertir a HTML usando opciones LowCode
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.html",
                        SaveFormat = SaveFormat.Html
                    });
            }

            Console.WriteLine("Conversions completed successfully.");
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


