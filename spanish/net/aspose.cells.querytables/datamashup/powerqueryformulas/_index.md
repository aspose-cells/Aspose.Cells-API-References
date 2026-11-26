---
title: "DataMashup.PowerQueryFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataMashup. Obtiene todas las fórmulas de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Obtiene todas las fórmulas de Power Query.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulasDemo
    {
        public static void Run()
        {
            // Cargar el libro de trabajo con fórmulas Power Query
            Workbook workbook = new Workbook("source.xlsx");
            
            // Obtener el objeto DataMashup
            DataMashup mashupData = workbook.DataMashup;
            
            // Verificar si hay alguna fórmula de Power Query
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // Iterar a través de cada fórmula de Power Query
                foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
                {
                    Console.WriteLine("Formula Definition:");
                    Console.WriteLine(formula.FormulaDefinition);
                    Console.WriteLine("----------------------");
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


