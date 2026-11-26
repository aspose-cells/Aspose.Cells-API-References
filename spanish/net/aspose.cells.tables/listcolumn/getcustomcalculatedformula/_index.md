---
title: "ListColumn.GetCustomCalculatedFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListColumn. Obtiene la fórmula de esta columna de lista"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

Obtiene la fórmula de esta columna de lista.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
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
    public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B1"].PutValue("Score");
            sheet.Cells["B2"].PutValue(85);
            sheet.Cells["B3"].PutValue(92);
            
            // Crear un objeto de lista
            int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = sheet.ListObjects[index];
            
            // Agregar una columna calculada
            ListColumn calcColumn = listObject.ListColumns[1];
            calcColumn.Formula = "=WEEKNUM([@Score])";
            
            // Obtener la fórmula calculada personalizada
            string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
            
            // Mostrar el resultado
            Console.WriteLine("Calculated Formula: " + formula);
        }
    }
}
```

### Ver también

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


