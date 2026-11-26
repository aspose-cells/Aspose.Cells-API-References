---
title: "Cell.IsDynamicArrayFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si la fórmula de la celda es una fórmula de matriz dinámica (true) o una fórmula de matriz heredada (false)"
type: docs
url: /es/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Indica si la fórmula de la celda es una fórmula de matriz dinámica (true) o una fórmula de matriz heredada (false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establezca una fórmula de matriz dinámica en la celda A1
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // Verifique si la celda contiene una fórmula de matriz dinámica
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // Guarda el libro de trabajo
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


