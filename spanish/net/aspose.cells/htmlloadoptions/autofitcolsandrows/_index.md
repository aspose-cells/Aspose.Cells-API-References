---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Indica si se ajustan automáticamente columnas y filas. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Indica si se ajustan automáticamente las columnas y filas. El valor predeterminado es false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Habilitar el ajuste automático de columnas y filas
            loadOptions.AutoFitColsAndRows = true;
            
            // Cargar archivo HTML con las opciones especificadas
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // El ajuste automático de columnas y filas se aplicará durante la carga
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


