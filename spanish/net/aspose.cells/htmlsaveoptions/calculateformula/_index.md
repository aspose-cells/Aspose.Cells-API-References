---
title: "HtmlSaveOptions.CalculateFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se deben calcular las fórmulas antes de guardar el archivo HTML"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/calculateformula/
---
## HtmlSaveOptions.CalculateFormula property

Indica si se deben calcular las fórmulas antes de guardar el archivo html.

```csharp
public bool CalculateFormula { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos y fórmulas a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Crear HtmlSaveOptions con CalculateFormula establecido en true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                CalculateFormula = true
            };

            // Guardar el libro de trabajo como HTML - las fórmulas se calcularán
            workbook.Save("HtmlWithCalculatedFormulas.html", saveOptions);

            Console.WriteLine("HTML file with calculated formulas created successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


