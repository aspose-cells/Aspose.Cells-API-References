---
title: "UnionRange.Merge"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnionRange. Combina un rango de celdas en una sola celda"
type: docs
url: /es/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

Combina un rango de celdas en una sola celda.

```csharp
public void Merge()
```

### Observaciones

Referencia la celda fusionada mediante la dirección de la celda superior izquierda del rango.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango de celdas (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // Colocar algunos datos en las celdas para visualizar la fusión
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // Crear un UnionRange a partir del Range
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // Llamar al método Merge
                unionRange.Merge();
                
                // Insertar valor en la celda fusionada
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // Descomenta para ver el efecto de descombinar
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


