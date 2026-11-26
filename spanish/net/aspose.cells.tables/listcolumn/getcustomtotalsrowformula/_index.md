---
title: "ListColumn.GetCustomTotalsRowFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListColumn. Obtiene la fórmula de la fila de totales de esta columna de lista"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/getcustomtotalsrowformula/
---
## ListColumn.GetCustomTotalsRowFormula method

Obtiene la fórmula de la fila de totales de esta columna de lista.

```csharp
public string GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Valor de retorno

La fórmula de esta columna de lista.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetCustomTotalsRowFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Establecer fórmula personalizada de totales
            ListColumn listColumn = listObject.ListColumns[0];
            listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Custom;
            listColumn.SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // Obtener y mostrar la fórmula personalizada de totales
            string formula = listColumn.GetCustomTotalsRowFormula(false, true);
            Console.WriteLine("Custom Totals Formula: " + formula);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


