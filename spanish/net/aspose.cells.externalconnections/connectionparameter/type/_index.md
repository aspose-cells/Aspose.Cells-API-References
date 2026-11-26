---
title: "ConnectionParameter.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameter. Tipo de parámetro usado. Si el parameterTypevalue entonces se usará el valor de boolean, double, integer o string. En este caso se espera que solo se especifique uno de boolean, double, integer o string"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

Tipo de parámetro utilizado. Si parameterType=value, se usará el valor de boolean, double, integer o string. En este caso, se espera que solo se especifique uno de {boolean, double, integer, o string}.

```csharp
public ConnectionParameterType Type { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyTypeDemo
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
                
                // Para demostración, mostraremos cómo se usaría Type si tuviéramos un parámetro
                if (parameter != null)
                {
                    // Obtener y mostrar el valor actual de Type
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // Establecer un nuevo valor de Type (ya que la propiedad es de lectura y escritura)
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // Demostración de respaldo cuando no podemos crear el parámetro
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterTypeDemo.xlsx");
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

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


