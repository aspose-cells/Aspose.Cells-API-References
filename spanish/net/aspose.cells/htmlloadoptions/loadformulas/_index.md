---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Indica si se importan fórmulas si el archivo html original contiene fórmulas"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

Indica si se importan fórmulas cuando el archivo html original contiene fórmulas

```csharp
public bool LoadFormulas { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // Crea una instancia de HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Establezca LoadFormulas a true para cargar fórmulas desde HTML
            loadOptions.LoadFormulas = true;

            // Cargue un archivo HTML que contiene fórmulas en un Workbook
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar la fórmula de la celda A1 (si está presente en HTML)
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


