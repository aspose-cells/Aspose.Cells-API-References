---
title: "CellArea.CompareTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellArea. Compara dos objetos CellArea según su esquina superior izquierda"
type: docs
url: /es/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

Compara dos objetos CellArea según su esquina superior izquierda.

```csharp
public int CompareTo(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto |  |

### Valor de retorno

Si dos esquinas están en filas diferentes, entonces compare sus índices de fila. De lo contrario, compare sus índices de columna. Si las dos esquinas son iguales, se devolverá 0.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // Cree dos objetos CellArea para la comparación
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // Demuestre el método CompareTo con el parámetro Object
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // Cree otra comparación con áreas iguales
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### Ver también

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


