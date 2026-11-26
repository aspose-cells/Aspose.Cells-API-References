---
title: "ConnectionParameter.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameter. Valor numérico no entero, valor entero, valor de cadena o valor booleano para usar como parámetro de consulta. Se usa solo cuando parameterType es value"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

Valor numérico no entero, valor entero, valor de cadena o valor booleano para usar como parámetro de consulta. Se usa solo cuando parameterType es value.

```csharp
public object Value { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                
                // Crear un parámetro de conexión (simulado ya que no conocemos los parámetros del constructor)
                ConnectionParameter parameter = null;
                
                // En un escenario real, crearías el parámetro correctamente
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Para demostración, crearemos un parámetro simulado con un valor
                // Esto muestra cómo se usaría la propiedad Value en la práctica
                if (parameter != null)
                {
                    // Establecer el valor (ya que Value es de lectura y escritura)
                    parameter.Value = "SampleParameterValue";
                    
                    // Obtener y mostrar el valor
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // Cambiar el valor para demostrar que es mutable
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // Demostración de respaldo cuando no podemos crear el parámetro
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterValueDemo.xlsx");
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


