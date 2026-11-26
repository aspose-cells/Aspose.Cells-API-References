---
title: "DBConnection.CommandType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. Especifica el tipo de comando OLE DB. 1. Query especifica un nombre de cubo 2. Query especifica una sentencia SQL 3. Query especifica un nombre de tabla 4. Query especifica que se ha proporcionado información predeterminada y depende del proveedor interpretarla. 5. Query se realiza contra un proveedor de datos de lista basado en la web"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Especifica el tipo de comando OLE DB. 1. La consulta especifica un nombre de cubo 2. La consulta especifica una instrucción SQL 3. La consulta especifica un nombre de tabla 4. La consulta indica que se ha proporcionado información predeterminada, y depende del proveedor interpretarla. 5. La consulta se realiza contra un proveedor de datos de lista basado en la web.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Inicializar un libro de trabajo (vacío o a partir de un archivo que pueda contener conexiones)
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
                    // Mostrar el valor actual de CommandType
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // Demostrar la configuración de CommandType (propiedad de lectura‑escritura)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Guardar el libro de trabajo (incluso si no ha cambiado) para ilustrar un flujo completo)
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


