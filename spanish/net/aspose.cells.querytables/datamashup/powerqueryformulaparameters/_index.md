---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataMashup. Obtiene los parámetros de fórmula de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Obtiene los parámetros de fórmula de Power Query.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad DataMashup.PowerQueryFormulas. Esta propiedad será eliminada 12 meses después a partir de noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulaParametersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la propiedad DataMashup
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Acceder a PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // Mostrar el recuento de parámetros
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // Iterar sobre los parámetros si existen
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


