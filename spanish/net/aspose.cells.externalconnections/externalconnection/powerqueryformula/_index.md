---
title: "ExternalConnection.PowerQueryFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Obtiene la definición de la fórmula Power Query"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Obtiene la definición de la fórmula de Power Query.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Cargar un libro de trabajo existente con conexiones de datos para demostrar PowerQueryFormula
            workbook = new Workbook("example.xlsx");
            
            // Acceder a una conexión existente (asumiendo que el libro de trabajo tiene al menos una conexión)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // Acceder a la propiedad PowerQueryFormula
                PowerQueryFormula powerQuery = connection.PowerQueryFormula;
                if (powerQuery != null)
                {
                    Console.WriteLine($"Formula Name: {powerQuery.Name}");
                    Console.WriteLine($"Formula Definition: {powerQuery.FormulaDefinition}");
                }
                else
                {
                    Console.WriteLine("No Power Query Formula found for this connection");
                }
            }
            else
            {
                Console.WriteLine("No data connections found in the workbook");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


