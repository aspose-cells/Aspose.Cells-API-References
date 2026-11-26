---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Convierte la fórmula A1 de la celda a la fórmula r1c1"
type: docs
url: /es/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Convierte la fórmula A1 de la celda a la fórmula r1c1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | La fórmula A1. |
| fila | Int32 | El índice de fila de la celda. |
| columna | Int32 | El índice de columna de la celda. |

### Valor de retorno

La fórmula R1C1.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Worksheet.ConvertFormulaReferenceStyle(). Esta propiedad será eliminada 12 meses después, a partir de agosto de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Convertir la fórmula de estilo A1 al estilo R1C1
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


