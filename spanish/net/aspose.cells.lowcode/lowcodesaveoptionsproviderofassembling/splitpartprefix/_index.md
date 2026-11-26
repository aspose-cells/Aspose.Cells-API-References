---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfAssembling. Prefijo para el índice de la parte dividida"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

Prefijo para el índice de la parte dividida.

```csharp
public string SplitPartPrefix { get; set; }
```

### Observaciones

Si solo hay una parte dividida y [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) es false, entonces este prefijo y el índice de la parte dividida (0) no se agregarán a la ruta del archivo resultante.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con datos que abarcan varias páginas
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // Configura la configuración de página para crear varias páginas
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // Inicializa el proveedor de opciones de guardado con la configuración de división
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // Guarda con el prefijo inicial (generará SplitResults/OriginalPart_0.pdf, etc.)
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // Modifica el prefijo de división
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Guarda con el prefijo modificado (generará SplitResults/ModifiedPart_0.pdf, etc.)
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


