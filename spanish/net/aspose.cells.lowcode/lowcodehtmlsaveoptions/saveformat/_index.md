---
title: "LowCodeHtmlSaveOptions.SaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeHtmlSaveOptions propiedad. Obtiene y establece el formato de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/
---
## LowCodeHtmlSaveOptions.SaveFormat property

Obtiene y establece el formato de la hoja de cálculo.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Observaciones

Al cambiar esta propiedad, el formato de guardado especificado por [`HtmlOptions`](../htmloptions/) será ignorado (si se había especificado antes).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            LowCodeHtmlSaveOptions options = new LowCodeHtmlSaveOptions();
            Console.WriteLine("Current SaveFormat value: " + options.SaveFormat);

            options.SaveFormat = SaveFormat.Html;
            options.HtmlOptions = new HtmlSaveOptions();

            workbook.Save("LowCodeHtmlExport.html", options.HtmlOptions);
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


