---
title: "TxtLoadOptions.HasFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Indica si el texto es una fórmula si comienza con"
type: docs
url: /es/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

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
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Crea opciones de carga de texto y habilita el análisis de fórmulas
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // Carga el libro de trabajo con fórmulas en el archivo de texto
            Workbook workbook = new Workbook("example.csv", options);
            
            // Accede a una celda con fórmula y muéstrala
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // Guarda el libro de trabajo
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


