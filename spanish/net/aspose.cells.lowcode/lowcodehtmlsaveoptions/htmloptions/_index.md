---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeHtmlSaveOptions propiedad. Las opciones generales para guardar html"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

Las opciones generales para guardar HTML.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### Observaciones

Cuando se especifica una instancia de [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/), el [`SaveFormat`](../saveformat/) será sobrescrito (si se había especificado antes).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // Crear opciones de guardado HTML de bajo código
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // Mostrar la configuración actual de exportación de líneas de cuadrícula
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // Guardar con líneas de cuadrícula visibles
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // Modificar opciones HTML para ocultar líneas de cuadrícula
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // Guardar sin líneas de cuadrícula
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


