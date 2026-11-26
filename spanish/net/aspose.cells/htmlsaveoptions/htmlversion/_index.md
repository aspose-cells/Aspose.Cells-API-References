---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Especifica la versión del estándar HTML que debe usarse al guardar en formato HTML. El valor predeterminado es HtmlVersion.Default"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

Especifica la versión del estándar HTML que debe usarse al guardar en formato HTML. El valor predeterminado es HtmlVersion.Default.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // Crear instancia de HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Mostrar valor actual de HtmlVersion
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // Establecer HtmlVersion a HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Guardar con versión HTML5
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // Cambiar a XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Guardar con versión XHTML
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // Restablecer a predeterminado
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // Guardar con versión predeterminada
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### Ver también

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


