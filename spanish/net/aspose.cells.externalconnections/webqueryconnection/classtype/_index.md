---
title: "WebQueryConnection.ClassType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de WebQueryConnection. Obtiene el tipo de este objeto ExternalConnection."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

Obtiene el tipo de este objeto [`ExternalConnection`](../../externalconnection/).

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyClassTypeDemo
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
                    // Muestra el valor de ClassType (propiedad de solo lectura)
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // Verifique el valor enum esperado para la consulta web.
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


