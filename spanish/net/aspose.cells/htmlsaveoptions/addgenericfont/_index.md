---
title: "HtmlSaveOptions.AddGenericFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se debe agregar una fuente genérica a la familia de fuentes CSS. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/addgenericfont/
---
## HtmlSaveOptions.AddGenericFont property

Indica si se debe agregar una fuente genérica a la familia de fuentes CSS. El valor predeterminado es true

```csharp
public bool AddGenericFont { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddGenericFontDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer texto de muestra con una fuente específica
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Pacifico";
            cell.SetStyle(style);

            // Guardar con AddGenericFont habilitado (predeterminado)
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            workbook.Save("output_with_generic.html", options);

            // Guardar con AddGenericFont deshabilitado
            options.AddGenericFont = false;
            workbook.Save("output_without_generic.html", options);

            // Verifique los resultados
            string withGeneric = File.ReadAllText("output_with_generic.html");
            string withoutGeneric = File.ReadAllText("output_without_generic.html");

            Console.WriteLine("With generic font: " + (withGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
            Console.WriteLine("Without generic font: " + (withoutGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


