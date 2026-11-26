---
title: "ExternalConnection.ReconnectionMethod"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/reconnectionmethod/
---
## ExternalConnection.ReconnectionMethod property

Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required.

```csharp
[Obsolete("Use ExternalConnection.ReconnectionMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ReConnectionMethodType ReconnectionMethod { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.ReconnectionMethodType. Esta propiedad será eliminada 12 meses después, desde octubre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Muestre el valor actual de ReconnectionMethod (operación de lectura)
                Console.WriteLine("Initial ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Establezca nuevos valores de ReconnectionMethod (ya que es de lectura-escritura)
                connection.ReconnectionMethod = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                connection.ReconnectionMethod = ReConnectionMethodType.Never;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Restablecer al valor predeterminado
                connection.ReconnectionMethod = ReConnectionMethodType.Required;
                Console.WriteLine("Reset ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("ReconnectionMethodDemo.xlsx");
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

* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


