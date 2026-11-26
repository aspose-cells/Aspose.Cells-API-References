---
title: "DBConnection.SecondCommand"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. Especifica una segunda cadena de texto de comando que se conserva cuando los campos de página basados en servidor de PivotTable están en uso. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command; no hay cláusula WHERE presente en la primera. Con base en estos 2 comandos, Command y ServerCommand, la interfaz de parámetros puede ser poblada y pueden construirse consultas parametrizadas"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE presente en la primera). Basado en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas

```csharp
public override string SecondCommand { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea una nueva instancia de DBConnection añadiéndola a la colección
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // Configura una conexión básica
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // Establece y demuestra la propiedad SecondCommand
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // Modifica SecondCommand para mostrar que es modificable
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // Guarda el libro de trabajo
                workbook.Save("SecondCommandDemo.xlsx");
                
                Console.WriteLine("SecondCommand demonstration completed successfully.");
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


