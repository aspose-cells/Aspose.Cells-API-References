---
title: "ExternalConnection.Credentials"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica el método de autenticación que se utilizará al establecer o restablecer la conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/credentials/
---
## ExternalConnection.Credentials property

Especifica el método de autenticación que se debe usar al establecer (o restablecer) la conexión.

```csharp
[Obsolete("Use ExternalConnection.CredentialsMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CredentialsMethodType Credentials { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad ExternalConnection.CredentialsMethodType. Esta propiedad será eliminada 12 meses después desde octubre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyCredentialsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor actual de Credentials
                Console.WriteLine("Initial Credentials value: " + connection.Credentials);
                
                // Establecer un nuevo valor de Credentials (ya que es de lectura-escritura)
                connection.Credentials = CredentialsMethodType.Integrated;
                Console.WriteLine("Updated Credentials value: " + connection.Credentials);
                
                // Recorrer los valores posibles
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    connection.Credentials = method;
                    Console.WriteLine($"Credentials set to: {method}");
                }
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("CredentialsDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


