---
title: "Cell.GetDependents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtenga todas las celdas cuya fórmula hace referencia a esta celda directamente"
type: docs
url: /es/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Obtén todas las celdas cuya fórmula hace referencia directa a esta celda.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAll | Booleano | Indica si se deben comprobar fórmulas en otras hojas de cálculo |

### Observaciones

Si una referencia que contiene esta celda aparece en la fórmula de otra celda, esa celda se considerará dependiente de esta celda, sin importar si la referencia o esta celda se utilizan o no durante el cálculo. Por ejemplo, aunque la celda A2 en la fórmula "=IF(TRUE,A1,A2)" no se use durante el cálculo, esta fórmula seguirá considerándose dependiente de A2. Para obtener esas fórmulas cuyos resultados calculados dependen de esta celda, utilice [`GetDependentsInCalculation`](../getdependentsincalculation/). Al rastrear dependientes de una celda, todas las fórmulas del libro o de la hoja de cálculo serán analizadas y verificadas. Por lo tanto, es un proceso que consume tiempo. Si el usuario necesita rastrear dependientes de muchas celdas, usar este método provocará un bajo rendimiento. Por consideraciones de rendimiento, el usuario debería usar [`GetDependentsInCalculation`](../getdependentsincalculation/) en su lugar. O, el usuario puede recopilar el mapa de precedentes de todas las celdas mediante [`GetPrecedents`](../getprecedents/) primero, y luego construir el mapa de dependientes según el mapa de precedentes.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer fórmulas que hacen referencia a B1
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Obtener todas las celdas que dependen de B1 (recursivo)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


