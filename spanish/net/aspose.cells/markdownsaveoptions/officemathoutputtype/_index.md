---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Indica cómo se exportan los objetos OfficeMath a Markdown. El valor predeterminado es Image"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

Indica cómo se exportan los objetos OfficeMath a Markdown, el valor predeterminado es Imagen.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra que incluyan una fórmula que pueda contener OfficeMath
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // Crear opciones de guardado Markdown
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Mostrar el valor actual de OfficeMathOutputType
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // Establecer OfficeMathOutputType a MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Guardar el libro de trabajo con tipo de salida MathML
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // Cambiar al tipo de salida Image
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Guardar el libro de trabajo con tipo de salida Image
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


