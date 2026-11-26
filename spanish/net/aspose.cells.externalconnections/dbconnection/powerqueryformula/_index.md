---
title: "DBConnection.PowerQueryFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. Obtiene la definición de la fórmula Power Query"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/powerqueryformula/
---
## DBConnection.PowerQueryFormula property

Obtiene la definición de la fórmula de Power Query.

```csharp
public override PowerQueryFormula PowerQueryFormula { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;

    public class DBConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la colección de conexiones externas
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Encontrar la primera DBConnection en la colección (si existe)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Acceder a la propiedad PowerQueryFormula (solo lectura)
                    PowerQueryFormula powerQueryFormula = dbConn.PowerQueryFormula;

                    if (powerQueryFormula != null)
                    {
                        // Mostrar las propiedades de PowerQueryFormula
                        Console.WriteLine("PowerQueryFormula Type: " + powerQueryFormula.Type);
                        Console.WriteLine("PowerQueryFormula GroupName: " + powerQueryFormula.GroupName);
                        Console.WriteLine("PowerQueryFormula FormulaDefinition: " + powerQueryFormula.FormulaDefinition);
                        Console.WriteLine("PowerQueryFormula Name: " + powerQueryFormula.Name);
                        Console.WriteLine("PowerQueryFormula Description: " + powerQueryFormula.Description);

                        // Demostrar el acceso a la colección PowerQueryFormulaItems
                        Console.WriteLine("Number of PowerQueryFormulaItems: " + powerQueryFormula.PowerQueryFormulaItems.Count);
                    }
                    else
                    {
                        Console.WriteLine("PowerQueryFormula is null for this connection.");
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved as PowerQueryFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


