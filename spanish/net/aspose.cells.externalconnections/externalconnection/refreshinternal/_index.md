---
title: "ExternalConnection.RefreshInternal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ExternalConnection property. Especifica el número de minutos entre actualizaciones automáticas de la conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

Especifica el número de minutos entre actualizaciones automáticas de la conexión.

```csharp
public int RefreshInternal { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // Crear una conexión de datos (usando la clase base ExternalConnection)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Establecer y mostrar la propiedad RefreshInternal
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // Modificar el intervalo de actualización
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // Guardar el libro de trabajo con la configuración de la conexión
                workbook.Save("RefreshInternalDemo.xlsx");
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


