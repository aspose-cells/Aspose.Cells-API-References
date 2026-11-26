---
title: "HtmlSaveOptions.PageTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. El título de la página html. Solo para guardar en un flujo html"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/pagetitle/
---
## HtmlSaveOptions.PageTitle property

El título de la página HTML. Solo para guardar en flujo HTML.

```csharp
public string PageTitle { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPageTitleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            // Establecer opciones de guardado HTML con PageTitle
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.PageTitle = "My Custom Page Title";

            // Guardar en HTML con el título especificado
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with custom page title: " + outputPath);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


