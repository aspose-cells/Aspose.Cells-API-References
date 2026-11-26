---
title: "WebQueryConnection.ConnectionFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. Obtiene el archivo de conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/connectionfile/
---
## WebQueryConnection.ConnectionFile property

Obtiene el archivo de conexión.

```csharp
public override string ConnectionFile { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Cree una hoja de cálculo de ejemplo con datos de consulta web
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Web Query Data";
                
                // Obtenga la primera conexión de consulta web existente (si la hay)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Muestre el valor de ConnectionFile (propiedad de solo lectura)
                    Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
                    
                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionFileDemo.xlsx");
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


