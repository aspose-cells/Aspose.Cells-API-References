---
title: "DataModelConnection.Command"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelConnection. La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa con el fin de recuperar datos"
type: docs
url: /es/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de DataModelConnection usando un objeto no inicializado
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Mostrar valor inicial de Command (vacío)
                Console.WriteLine("Initial Command: " + connection.Command);

                // Establecer la propiedad Command
                connection.Command = "SELECT * FROM Customers";
                
                // Mostrar el valor actualizado de Command
                Console.WriteLine("Updated Command: " + connection.Command);

                // Establecer otras propiedades requeridas para una conexión completa
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Guardar el libro de trabajo con la conexión
                workbook.Save("CommandDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


