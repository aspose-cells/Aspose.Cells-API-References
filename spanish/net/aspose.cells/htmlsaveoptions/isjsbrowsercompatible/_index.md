---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si JavaScript es compatible con navegadores que no soportan JavaScript. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

Indica si JavaScript es compatible con navegadores que no soportan JavaScript. El valor predeterminado es true.

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // Configurar opciones de guardado HTML con IsJsBrowserCompatible establecido en true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // Guardar el libro con compatibilidad JavaScript
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


