---
title: "ListColumn.SetCustomTotalsRowFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListColumn. Obtiene la fórmula de la fila de totales de esta columna de lista"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

Obtiene la fórmula de la fila de totales de esta columna de lista.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | la fórmula de esta columna de lista. |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Habilitar la fila de totales y establecer una fórmula personalizada
            listObject.ShowTotals = true;
            listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

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


