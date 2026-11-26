---
title: "WebQueryConnection.Url"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. URL a usar para actualizar datos externos"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

URL a usar para actualizar datos externos.

```csharp
public string Url { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una conexión de consulta web añadiéndola a la colección
            // Es probable que la colección cree y devuelva el objeto de conexión
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // Establecer la URL inicial para la consulta web
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // Cambiar la URL a una fuente diferente
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // Configurar la conexión para analizar datos XML
            connection.IsXml = true;

            // Actualizar la conexión de datos (normalmente recuperaría datos de la URL)
            // Nota: El acceso web real requeriría conectividad de red
            // workbook.RefreshAllConnections();

            // Guardar el libro con la conexión de consulta web
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


