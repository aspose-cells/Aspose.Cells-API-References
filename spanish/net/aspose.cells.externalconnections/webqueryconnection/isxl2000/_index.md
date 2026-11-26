---
title: "WebQueryConnection.IsXl2000"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de WebQueryConnection. Esta bandera existe por compatibilidad con versiones anteriores de archivos de hoja de cálculo existentes y se establece en true si esta consulta web se actualizó en una aplicación de hoja de cálculo más reciente o igual a Microsoft Excel 2000. Este es un atributo opcional que puede ser ignorado."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

Esta bandera existe por compatibilidad hacia atrás con archivos de hoja de cálculo más antiguos existentes, y se establece en true si esta consulta web se actualizó en una aplicación de hoja de cálculo más reciente o igual a Microsoft Excel 2000. Este es un atributo opcional que puede ser ignorado.

```csharp
public bool IsXl2000 { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la primera conexión de consulta web existente (si la hay)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Muestre el valor inicial de IsXl2000.
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // Establezca IsXl2000 en true (ya que es de lectura-escritura).
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // Restablezca IsXl2000 a false.
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
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


