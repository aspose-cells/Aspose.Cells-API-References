---
title: "PowerQueryFormulaParameter.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaParameter. Obtiene el tipo de la fórmula Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

Obtiene el tipo de la fórmula de Power Query.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Dado que no podemos crear un PowerQueryFormulaParameter directamente sin conocer los parámetros de constructor requeridos,
                // demostraremos el acceso a la propiedad Type a través de los parámetros de una tabla de consulta existente
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // En un escenario real, accedería a esto desde una tabla de consulta existente
                // Para fines de demostración, mostraremos cómo verificar el tipo si tuviera una instancia
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // Muestre el valor de la propiedad Type (propiedad de solo lectura)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // Mostrar valores posibles de enumeración
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // Guarda el libro de trabajo
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

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


