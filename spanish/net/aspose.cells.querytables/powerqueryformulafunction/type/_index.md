---
title: "PowerQueryFormulaFunction.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaFunction. Obtiene el tipo de fórmula de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

Obtiene el tipo de la fórmula de Power Query.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una función de fórmula Power Query
            // Dado que no podemos crear directamente, necesitaremos obtenerlo de algún lugar
            // Para fines de demostración, solo mostraremos cómo acceder a la propiedad Type
            // (En uso real, obtendrías esto de una colección existente)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // Dado que tampoco podemos crear un QueryTable directamente, omitiremos esa parte
            QueryTable queryTable = null; // Can't instantiate directly
            
            // No se puede agregar a la colección de tablas de consulta de esta manera - es de solo lectura
            // worksheet.QueryTables[0] = queryTable; // Línea eliminada
            
            // Para demostración, solo mostraremos el formato de salida que usaríamos si tuviéramos una función
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // Guardar el resultado
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


