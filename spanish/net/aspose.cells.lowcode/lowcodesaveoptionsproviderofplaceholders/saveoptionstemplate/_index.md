---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfPlaceHolders propiedad. La plantilla para crear una instancia de opciones de guardado en GetSaveOptions"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate property

La plantilla para crear una instancia de opciones de guardado en [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Observaciones

Si la plantilla ha sido especificada, entonces la instancia creada copiará todas las configuraciones de ella y actualizará el archivo de salida en consecuencia.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            
            // Inicializar el proveedor con una plantilla de ruta que contiene marcadores de posición
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/Sheet_{sheet}_Part_{part}.pdf");
            
            // Mostrar el estado inicial de la plantilla
            Console.WriteLine($"Initial SaveOptionsTemplate: {(provider.SaveOptionsTemplate == null ? "Not set" : "Configured")}");
            
            // Crear y configurar una nueva plantilla de opciones de guardado
            provider.SaveOptionsTemplate = new LowCodePdfSaveOptions
            {
                PdfOptions = new PdfSaveOptions  // Fixed property name from PdfSaveOptions to PdfOptions
                {
                    Compliance = PdfCompliance.PdfA1a,
                    ExportDocumentStructure = true
                }
            };

            // Configurar parámetros de división
            provider.BuildPathWithSheetAlways = true;
            provider.SplitPartPrefix = "Split_";
            
            // Mostrar opciones PDF configuradas
            var pdfOptions = (LowCodePdfSaveOptions)provider.SaveOptionsTemplate;
            Console.WriteLine($"Configured PDF Compliance: {pdfOptions.PdfOptions.Compliance}");  // Fixed property access
            Console.WriteLine($"Document Structure Export: {pdfOptions.PdfOptions.ExportDocumentStructure}");  // Fixed property access

            // Agregar salto de página para crear partes divididas
            worksheet.HorizontalPageBreaks.Add(0);
            
            // Guardar usando la configuración del proveedor (la división/guardado real ocurriría aquí)
            Console.WriteLine("Workbook prepared with SaveOptionsTemplate configuration");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


