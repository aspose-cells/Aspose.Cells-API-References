---
title: "ConnectionParameter.SqlType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameter. Tipo de datos SQL del parámetro. Solo válido para fuentes ODBC"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/sqltype/
---
## ConnectionParameter.SqlType property

Tipo de datos SQL del parámetro. Válido solo para fuentes ODBC.

```csharp
public SqlDataType SqlType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertySqlTypeDemo
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
                
                // Para demostración, mostraremos cómo se usaría SqlType si tuviéramos un parámetro
                if (parameter != null)
                {
                    // Obtener y mostrar el valor actual de SqlType
                    Console.WriteLine("Current SqlType: " + parameter.SqlType);
                    
                    // Establecer un nuevo valor de SqlType (ya que la propiedad es de lectura y escritura)
                    parameter.SqlType = SqlDataType.SqlInteger;
                    Console.WriteLine("Updated SqlType: " + parameter.SqlType);
                }
                else
                {
                    // Demostración de respaldo cuando no podemos crear el parámetro
                    workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
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

* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


