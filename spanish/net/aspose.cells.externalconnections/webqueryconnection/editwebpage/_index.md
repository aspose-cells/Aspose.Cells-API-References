---
title: "WebQueryConnection.EditWebPage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. La URL de la página web orientada al usuario que muestra los datos de la consulta web. Esta URL se conserva en caso de que sourceDatatrue y url hayan sido redirigidos para referenciar un archivo XML. Entonces la página orientada al usuario puede mostrarse en la UI y los datos XML pueden recuperarse en segundo plano."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

La URL de la página web orientada al usuario que muestra los datos de la consulta web. Esta URL se conserva en el caso de que sourceData="true" y la url haya sido redirigida para referenciar un archivo XML. Entonces la página orientada al usuario puede mostrarse en la interfaz y los datos XML pueden recuperarse en segundo plano.

```csharp
public string EditWebPage { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a la primera conexión de consulta web existente (si la hay)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Establezca el valor inicial de EditWebPage
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // Actualice el valor de EditWebPage
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // Guardar el libro con la conexión de consulta web
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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


