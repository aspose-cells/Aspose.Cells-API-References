---
title: "WebQueryConnection.IsConsecutive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. Indicador que muestra si los delimitadores consecutivos deben tratarse como un solo delimitador"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

Indicador que indica si los delimitadores consecutivos deben tratarse como un solo delimitador.

```csharp
public bool IsConsecutive { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Cree una conexión de consulta web accediendo a la primera conexión
            // (suponiendo que haya al menos una conexión disponible)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // Muestre el valor inicial de IsConsecutive (predeterminado)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // Establezca IsConsecutive a true
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // Restablezca IsConsecutive a false
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // Guardar el libro con la conexión de consulta web
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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


