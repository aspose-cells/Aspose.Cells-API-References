---
title: "WebQueryConnection.IsXml"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. true si la fuente de la consulta web es XML en lugar de HTML, de lo contrario false"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/isxml/
---
## WebQueryConnection.IsXml property

true si la fuente de la consulta web es XML (en lugar de HTML), de lo contrario false.

```csharp
public bool IsXml { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a la primera conexión de datos (asumiendo que es una WebQueryConnection)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Mostrar el valor inicial de IsXml
                    Console.WriteLine("Initial IsXml value: " + connection.IsXml);
                    
                    // Establecer IsXml a true (ya que es de lectura-escritura)
                    connection.IsXml = true;
                    Console.WriteLine("Updated IsXml value: " + connection.IsXml);
                    
                    // Restablecer IsXml a false
                    connection.IsXml = false;
                    Console.WriteLine("Final IsXml value: " + connection.IsXml);
                    
                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionIsXmlDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
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


