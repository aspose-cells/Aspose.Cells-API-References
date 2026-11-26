---
title: "DataModelConnection.ConnectionString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelConnection. La cadena de información de conexión se utiliza para establecer contacto con una fuente de datos OLE DB o ODBC"
type: docs
url: /es/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

La cadena de información de conexión se usa para contactar con una fuente de datos OLE DB o ODBC.

```csharp
public override string ConnectionString { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
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

                // Mostrar el valor inicial de ConnectionString (vacío)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // Establecer la propiedad ConnectionString
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // Muestra el valor actualizado de ConnectionString
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // Establecer otras propiedades requeridas para una conexión completa
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // Guardar el libro de trabajo con la conexión
                workbook.Save("ConnectionStringDemo.xlsx");
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


