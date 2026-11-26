---
title: "Cell.Formula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene o establece una fórmula de la Celda"
type: docs
url: /es/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Obtiene o establece una fórmula de la [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### Observaciones

Una cadena de fórmula siempre comienza con un signo igual (=). Y por favor, siempre use la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca valores en las celdas que se usarán en la fórmula
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // Establezca la fórmula en la celda B6
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // Calcular la fórmula
            workbook.CalculateFormula();

            // Mostrar el resultado
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


