---
title: "HtmlSaveOptions.ExportFrameScriptsAndProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan los scripts de marco y las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Indica si se exportan scripts de marco y propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFrameScriptsAndPropertiesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Establecer opciones de guardado HTML con ExportFrameScriptsAndProperties
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportFrameScriptsAndProperties = true;

            // Guardar como HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportFrameScriptsAndProperties enabled.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


