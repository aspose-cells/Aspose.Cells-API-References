---
title: "Cell.GetDependentsInCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene todas las celdas cuyo resultado calculado depende de esta celda"
type: docs
url: /es/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Obtiene todas las celdas cuyo resultado calculado depende de esta celda.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recursivo | Booleano | Devuelve los dependientes que no hacen referencia a esta celda directamente, sino a otras hojas de esta celda. |

### Valor de retorno

Enumerador para enumerar todos los dependientes (objetos Cell)

### Observaciones

Para usar este método, asegúrese de que el libro de trabajo tenga el valor verdadero para [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) y haya sido calculado completamente con esta configuración. Si no hay ninguna referencia de fórmula a esta celda, se devolverá null.

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
            Console.WriteLine("B1's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
            
            en = cells["B2"].GetDependentsInCalculation(false);
            Console.WriteLine("B2's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


