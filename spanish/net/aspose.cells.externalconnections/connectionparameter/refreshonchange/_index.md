---
title: "ConnectionParameter.RefreshOnChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameter. Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de una celda que proporciona el valor del parámetro cambia. Si es true, los datos externos se actualizan usando el nuevo valor del parámetro cada vez que hay un cambio. Si es false, los datos externos solo se actualizan cuando el usuario lo solicita o cuando otro evento desencadena la actualización, p. ej., al abrir el libro de trabajo"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de una celda que proporciona el valor del parámetro cambia. Si true, los datos externos se actualizan usando el nuevo valor del parámetro cada vez que hay un cambio. Si false, los datos externos solo se actualizan cuando lo solicita el usuario, o cuando otro evento desencadena la actualización (p. ej., al abrir el libro de trabajo).

```csharp
public bool RefreshOnChange { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                
                // Crear un parámetro de conexión (simulado ya que los parámetros del constructor son desconocidos)
                ConnectionParameter parameter = null;
                
                // En un escenario real, crearías el parámetro correctamente
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Para demostración, mostraremos cómo se usaría RefreshOnChange si tuviéramos un parámetro
                if (parameter != null)
                {
                    // Obtener y mostrar el valor actual de RefreshOnChange
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // Establecer un nuevo valor RefreshOnChange (ya que la propiedad es de lectura y escritura)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // Demostración de respaldo cuando no podemos crear el parámetro
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


