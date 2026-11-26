---
title: "ExternalConnection.SSOId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Identificador para Single Sign On (SSO) utilizado para la autenticación entre un servidor intermedio de spreadsheetML y la fuente de datos externa"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

Identificador para Single Sign On (SSO) usado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa.

```csharp
public string SSOId { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySSOIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a la primera conexión externa
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor inicial de SSOId (probablemente nulo para una conexión nueva)
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // Establecer un nuevo valor de SSOId (ya que es de lectura-escritura)
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // Borrar el SSOId
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("SSOIdDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


