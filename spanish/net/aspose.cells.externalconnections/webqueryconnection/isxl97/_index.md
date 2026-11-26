---
title: "WebQueryConnection.IsXl97"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de WebQueryConnection. Esta bandera existe por compatibilidad con versiones anteriores de archivos de hoja de cálculo existentes y se establece en true si esta consulta web se creó en Microsoft Excel 97. Este es un atributo opcional que puede ser ignorado."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

Esta bandera existe por compatibilidad hacia atrás con archivos de hoja de cálculo más antiguos existentes, y se establece en true si esta consulta web se creó en Microsoft Excel 97. Este es un atributo opcional que puede ser ignorado.

```csharp
public bool IsXl97 { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Cree una hoja de cálculo con algunos datos para que el ejemplo tenga sentido.
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // Cree una conexión de consulta web cargándola desde un archivo existente o creándola correctamente.
                // Dado que no podemos crear WebQueryConnection directamente, accederemos a una existente.
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Muestre el valor inicial de IsXl97.
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // Establezca IsXl97 en true (ya que es de lectura-escritura).
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // Restablezca IsXl97 a false.
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // Guarda el libro de trabajo
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
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


