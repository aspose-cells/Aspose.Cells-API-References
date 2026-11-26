---
title: "ExternalConnection.IsDeleted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ExternalConnection property. Indica si la conexión del libro de trabajo asociada ha sido eliminada. verdadero si la conexión ha sido eliminada, de lo contrario falso"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/isdeleted/
---
## ExternalConnection.IsDeleted property

Indica si la conexión del libro de trabajo asociada ha sido eliminada. true si la conexión ha sido eliminada; de lo contrario, false.

```csharp
public bool IsDeleted { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor inicial de IsDeleted
                Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
                
                // Alternar el valor de IsDeleted (ya que es de lectura-escritura)
                connection.IsDeleted = !connection.IsDeleted;
                Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("IsDeletedDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


