---
title: "WebQueryConnection.IsXmlSourceData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. Indicador que muestra que los datos de origen XML deben importarse en lugar de la tabla HTML misma"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/
---
## WebQueryConnection.IsXmlSourceData property

Bandera que indica que los datos de origen XML deben importarse en lugar de la tabla HTML misma.

```csharp
public bool IsXmlSourceData { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlSourceDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a una conexión de consulta web existente o crear una mediante la inicialización adecuada
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Mostrar el valor inicial de IsXmlSourceData
                    Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Establecer IsXmlSourceData a true
                    connection.IsXmlSourceData = true;
                    Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Restablecer IsXmlSourceData a false
                    connection.IsXmlSourceData = false;
                    Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionIsXmlSourceDataDemo.xlsx");
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


