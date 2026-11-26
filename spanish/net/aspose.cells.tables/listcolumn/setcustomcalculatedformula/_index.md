---
title: "ListColumn.SetCustomCalculatedFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListColumn. Establece la fórmula para esta columna de lista"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/setcustomcalculatedformula/
---
## ListColumn.SetCustomCalculatedFormula method

Establece la fórmula para esta columna de lista.

```csharp
public void SetCustomCalculatedFormula(string formula, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | la fórmula de esta columna de lista. |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnMethodSetCustomCalculatedFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para la tabla
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Total");

            // Crear tabla
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true); // Adjusted parameters to match correct overload
            ListObject table = worksheet.ListObjects[tableIndex];

            // Obtener la segunda columna de lista
            ListColumn totalColumn = table.ListColumns[1];

            try
            {
                // Establecer fórmula personalizada usando notación A1 con la configuración regional estándar
                totalColumn.SetCustomCalculatedFormula("=A2*1.1", false, false);
                
                Console.WriteLine("Custom formula set successfully.");
                Console.WriteLine($"Cell B2 formula: {worksheet.Cells["B2"].Formula}");
                Console.WriteLine($"Cell B3 formula: {worksheet.Cells["B3"].Formula}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("SetCustomCalculatedFormulaExample.xlsx");
        }
    }
}
```

### Ver también

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


