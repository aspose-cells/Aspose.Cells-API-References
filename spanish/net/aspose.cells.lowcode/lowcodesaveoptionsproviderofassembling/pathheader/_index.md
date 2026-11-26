---
title: "LowCodeSaveOptionsProviderOfAssembling.PathHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling propiedad. Encabezado antes del contenido añadido de la hoja y parte dividida de la ruta del archivo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/
---
## LowCodeSaveOptionsProviderOfAssembling.PathHeader property

Parte de encabezado (antes del contenido añadido de la hoja y la parte dividida) de la ruta del archivo.

```csharp
public string PathHeader { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathHeaderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos que se dividirán en múltiples partes
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 150; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Inicializar el proveedor de opciones de guardado con valores predeterminados
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/QuarterlyReport_",
                PathTail = ".html",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions() // Changed from HtmlSaveOptions to LowCodeSaveOptions
            };

            Console.WriteLine($"Initial PathHeader: {provider.PathHeader}");

            // Modificar la configuración de la ruta
            provider.PathHeader = "output/ModifiedReport_";
            provider.SheetPrefix = "Sheet_";
            provider.SplitPartPrefix = "Part_";

            // Demostrar el efecto guardando con la configuración actual del proveedor
            workbook.Save("result.html", SaveFormat.Html); // Changed second parameter to SaveFormat.Html

            Console.WriteLine("Check 'output' directory for split files named like 'ModifiedReport_Sheet_0_Part_0.html'");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


