---
title: "UnionRange.UnMerge"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnionRange. Desfusiona celdas fusionadas de este rango"
type: docs
url: /es/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

Descombina celdas combinadas de este rango.

```csharp
public void UnMerge()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango y fusionar celdas
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // Fusionar las celdas y colocar un valor
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // Llamar al método UnMerge
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // Colocar valores en las celdas desfusionadas para demostrar el efecto
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


