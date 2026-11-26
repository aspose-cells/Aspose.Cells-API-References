---
title: "WebQueryConnection.EditPage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. La URL de la página web orientada al usuario que muestra los datos de la consulta web. Esta URL se conserva en caso de que sourceDatatrue y url hayan sido redirigidos para referenciar un archivo XML. Entonces la página orientada al usuario puede mostrarse en la UI y los datos XML pueden recuperarse en segundo plano."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

La URL de la página web orientada al usuario que muestra los datos de la consulta web. Esta URL se conserva en el caso de que sourceData="true" y la url haya sido redirigida para referenciar un archivo XML. Entonces la página orientada al usuario puede mostrarse en la interfaz y los datos XML pueden recuperarse en segundo plano.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad WebQueryConnection.EditWebPage. Esta propiedad será eliminada 12 meses después, desde octubre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión de consulta web existente si está disponible
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Mostrar el valor inicial de EditPage
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // Establecer EditPage a una nueva URL (ya que es de lectura-escritura)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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


