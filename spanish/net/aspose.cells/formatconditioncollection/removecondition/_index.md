---
title: "FormatConditionCollection.RemoveCondition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatConditionCollection. Elimina la condición de formato por índice"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

Elimina la condición de formato por índice.

```csharp
public void RemoveCondition(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de la condición de formato que se eliminará. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la colección de condiciones de formato
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // Agregar algunas condiciones de ejemplo
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // Mostrar el recuento inicial
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // Eliminar la primera condición
                formatConditions.RemoveCondition(index1);
                
                // Mostrar recuento actualizado
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // Guarda el libro de trabajo
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


