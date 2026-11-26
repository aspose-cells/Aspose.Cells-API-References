---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet método. Convierte el estilo de referencia de la fórmula"
type: docs
url: /es/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Convierte el estilo de referencia de la fórmula.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | La fórmula a convertir. |
| toR1C1 | Booleano | ¿A qué estilo de referencia convertir la fórmula? Si la fórmula original está en estilo de referencia A1, entonces este valor debe ser verdadero para que la fórmula se convierta de A1 a estilo de referencia R1C1; si la fórmula original está en estilo de referencia R1C1, entonces este valor debe ser falso para que la fórmula se convierta de R1C1 a estilo A1; |
| baseCellRow | Int32 | El índice de fila de la celda base. |
| baseCellColumn | Int32 | El índice de columna de la celda base. |

### Valor de retorno

La fórmula convertida.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Ejemplo 1: Convertir estilo R1C1 a estilo A1
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // Ejemplo 2: Convertir con referencias mixtas
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


