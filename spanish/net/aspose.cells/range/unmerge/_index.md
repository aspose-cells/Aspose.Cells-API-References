---
title: "Range.UnMerge"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Descombina celdas combinadas de este rango"
type: docs
url: /es/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Descombina celdas combinadas de este rango.

```csharp
public void UnMerge()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Combinar celdas B2 a D4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // Verificar si la celda B2 está combinada antes de descombinar
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // Descombinar el rango
            range.UnMerge();
            
            // Verificar si la celda B2 está combinada después de descombinar
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


