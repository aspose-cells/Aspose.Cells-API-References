---
title: "HtmlSaveOptions.IsFullPathLink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se utiliza un enlace de ruta completa en sheet00x.htmfilelist.xml y tabstrip.htm. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

Indica si se utiliza una ruta completa en los enlaces de sheet00x.htm, filelist.xml y tabstrip.htm. El valor predeterminado es false.

```csharp
public bool IsFullPathLink { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Demostrar la propiedad IsFullPathLink
            saveOptions.IsFullPathLink = true; // Set to true to use full path links
            
            // Guardar con diferentes configuraciones de IsFullPathLink
            workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
            
            saveOptions.IsFullPathLink = false; // Set to false for relative paths
            workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


