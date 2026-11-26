---
title: "WebQueryConnection.IsSameSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de WebQueryConnection. Bandera que indica si se deben analizar todas las tablas dentro de un bloque PRE con la misma configuración de ancho que la primera fila."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

Indicador que indica si se deben analizar todas las tablas dentro de un bloque PRE con la misma configuración de ancho que la primera fila.

```csharp
public bool IsSameSettings { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
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
                    // Muestre el valor inicial de IsSameSettings
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Establezca IsSameSettings a true (ya que es de lectura-escritura)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Restablezca IsSameSettings a false
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
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


