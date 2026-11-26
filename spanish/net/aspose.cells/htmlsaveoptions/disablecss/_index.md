---
title: "HtmlSaveOptions.DisableCss"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si solo se aplican estilos en línea sin depender de CSS. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

Indica si solo se aplican estilos en línea, sin depender de CSS. El valor predeterminado es false.

```csharp
public bool DisableCss { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo y formato
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // Crear instancia de HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Mostrar el valor actual de DisableCss
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // Establecer DisableCss en true (usando estilos en línea en lugar de CSS)
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // Establecer DisableCss en false (usando estilos CSS)
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // Comparar los archivos de salida para ver la diferencia en el enfoque de estilo
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


