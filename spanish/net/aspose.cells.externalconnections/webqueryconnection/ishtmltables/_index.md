---
title: "WebQueryConnection.IsHtmlTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. Indicador que muestra si las consultas web deben trabajar solo con tablas HTML"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/ishtmltables/
---
## WebQueryConnection.IsHtmlTables property

Indicador que indica si las consultas web deben funcionar solo en tablas HTML.

```csharp
public bool IsHtmlTables { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsHtmlTablesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Crear una conexión de consulta web mediante el indexador de la colección
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

                Console.WriteLine("Initial IsHtmlTables: " + connection.IsHtmlTables);
                
                connection.IsHtmlTables = true;
                Console.WriteLine("Updated IsHtmlTables: " + connection.IsHtmlTables);

                workbook.Save("IsHtmlTablesDemo.xlsx");
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


