---
title: "HtmlSaveOptions.IsIECompatible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "HtmlSaveOptions propiedad. Indica si el HTML de salida es compatible con el navegador IE. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

Indica si el HTML de salida es compatible con el navegador IE. El valor predeterminado es false

```csharp
public bool IsIECompatible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsIECompatibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("HTML Export Demo");

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer la propiedad IsIECompatible
            saveOptions.IsIECompatible = false; // Disable IE compatibility mode
            
            // Guardar el libro de trabajo con opciones HTML
            workbook.Save("HtmlExportDemo.html", saveOptions);

            Console.WriteLine("HTML file saved with IsIECompatible = false");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


