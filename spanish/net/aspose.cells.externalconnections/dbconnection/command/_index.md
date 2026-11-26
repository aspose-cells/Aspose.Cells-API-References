---
title: "DBConnection.Command"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

La cadena que contiene el comando de base de datos que se pasa a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos

```csharp
public override string Command { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyCommandDemo
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
                    // Mostrar el valor actual de Command (operación de lectura)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Demostrar la configuración de Command (propiedad de lectura‑escritura)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Guarda el libro de trabajo
                workbook.Save("CommandDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandDemo.xlsx");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


