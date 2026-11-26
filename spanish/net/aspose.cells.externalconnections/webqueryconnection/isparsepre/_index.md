---
title: "WebQueryConnection.IsParsePre"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. Indicador que muestra si los datos contenidos dentro de etiquetas HTML PRE en la página web se analizan en columnas al importar la página a una tabla de consulta"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

Indicador que indica si los datos contenidos dentro de etiquetas HTML PRE en la página web se analizan en columnas al importar la página a una tabla de consulta.

```csharp
public bool IsParsePre { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Cree una nueva conexión de consulta web usando la conexión existente del libro de trabajo
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // Muestre el valor inicial de IsParsePre (predeterminado)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // Establezca IsParsePre a true
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // Restablecer IsParsePre a false
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // Guarda el libro de trabajo
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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


