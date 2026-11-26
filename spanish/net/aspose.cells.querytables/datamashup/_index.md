---
title: "Clase DataMashup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.QueryTables.DataMashup. Representa datos de mashup"
type: docs
url: /es/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

Representa datos mashup.

```csharp
public class DataMashup
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Obsoleto.**) Obtiene los parámetros de la fórmula de Power Query. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Obtiene todas las fórmulas de Power Query. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class DataMashupDemo
    {
        public static void DataMashupExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la propiedad DataMashup del libro de trabajo
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // Acceder a la propiedad PowerQueryFormulas
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Acceder a la propiedad PowerQueryFormulaParameters
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Ejemplo de uso: Iterar a través de PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Ejemplo de uso: iterar a través de PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Guarda el libro de trabajo
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


