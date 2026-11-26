---
title: "ExternalConnection.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Obtiene o establece el tipo de origen de datos de la conexión externa"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/type/
---
## ExternalConnection.Type property

Obtiene o establece el tipo de DataSource de la conexión externa.

```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.SourceType. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor actual de Type (operación de lectura)
                Console.WriteLine("Initial Type value: " + connection.Type);
                
                // Establecer un nuevo valor de Type (ya que es de lectura‑escritura)
                connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
                Console.WriteLine("Updated Type value: " + connection.Type);
                
                // Recorrer los valores posibles para demostrar la capacidad de configuración
                foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
                {
                    if ((int)type != 102) // Skip duplicate enum value
                    {
                        connection.Type = type;
                        Console.WriteLine($"Type set to: {type}");
                    }
                }
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("TypeDemo.xlsx");
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


