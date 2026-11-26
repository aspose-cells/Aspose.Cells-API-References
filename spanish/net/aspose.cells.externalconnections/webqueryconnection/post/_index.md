---
title: "WebQueryConnection.Post"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. Devuelve o establece la cadena utilizada con el método post para enviar datos a un servidor web y obtener datos de una consulta web"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

Devuelve o establece la cadena utilizada con el método post para enviar datos a un servidor web y obtener datos de una consulta web.

```csharp
public string Post { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una conexión de consulta web accediendo a una existente o creando mediante la inicialización adecuada
                // Dado que no podemos instanciar directamente WebQueryConnection, usaremos la primera conexión si existe
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // Si no existen conexiones, demostraremos con una conexión simulada
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // Establecer el valor inicial de Post
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // Modificar el valor de Post
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // Borrar el valor de Post
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // Guarda el libro de trabajo
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


