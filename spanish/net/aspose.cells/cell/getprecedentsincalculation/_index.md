---
title: "Cell.GetPrecedentsInCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene todas las referencias precedentes a celdas en el libro actual utilizadas por la fórmula de esta celda al calcularla"
type: docs
url: /es/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Obtiene todos los precedentes (referencia a celdas en el libro actual) utilizados por la fórmula de esta celda al calcularla.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Valor de retorno

Enumerador para enumerar todas las referencias (ReferredArea)

### Observaciones

Este método solo puede funcionar cuando [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) es verdadero para el libro y el libro ha sido calculado completamente. Si esta celda no es una fórmula o no hace referencia a ninguna otra celda, se devolverá null.

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsInCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["B1"].PutValue(10);
            cells["B2"].PutValue(20);
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
            Console.WriteLine("A2's calculation precedents:");
            while(en.MoveNext())
            {
                ReferredArea r = (ReferredArea)en.Current;
                Console.WriteLine(r);
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


