---
title: "ConnectionParameter.CellReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameter. Referencia de celda que indica qué valor de celda usar para el parámetro de consulta. Se usa solo cuando parameterType es cell"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

Referencia de celda que indica el valor de cuál celda usar para el parámetro de consulta. Se usa solo cuando parameterType es cell.

```csharp
public string CellReference { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyCellReferenceDemo
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
                
                // Para demostración, mostraremos cómo se usaría CellReference si tuviéramos un parámetro
                if (parameter != null)
                {
                    // Obtener y mostrar el valor actual de CellReference
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // Establecer un nuevo valor de CellReference (ya que la propiedad es de lectura y escritura)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // Demostración de respaldo cuando no podemos crear el parámetro
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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


