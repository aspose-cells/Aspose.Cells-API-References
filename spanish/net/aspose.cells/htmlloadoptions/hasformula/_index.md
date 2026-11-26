---
title: "HtmlLoadOptions.HasFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Indica si el texto es una fórmula si comienza con"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Indica si el texto es una fórmula si comienza con "=".

```csharp
public bool HasFormula { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Establezca HasFormula a false para tratar las cadenas de fórmula como texto plano
            loadOptions.HasFormula = false;
            
            // Crear workbook con archivo HTML y opciones de carga
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Mostrar algunos valores de celdas para demostrar la importación de HTML
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // Guardar como XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


