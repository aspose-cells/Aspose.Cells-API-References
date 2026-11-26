---
title: "DBConnection.ClassType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. Obtiene el tipo de este objeto ExternalConnection"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

Obtiene el tipo de este objeto [`ExternalConnection`](../../externalconnection/).

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea una nueva instancia de DBConnection añadiéndola a la colección
                // Dado que DBConnection no tiene un constructor público sin parámetros,
                // dejaremos que la colección lo cree por nosotros
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // Muestra el valor de ClassType (propiedad de solo lectura)
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // Demuestra la configuración de otras propiedades para que el ejemplo sea más significativo
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // Guarda el libro de trabajo
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


