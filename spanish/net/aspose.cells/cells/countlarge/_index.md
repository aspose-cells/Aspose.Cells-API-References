---
title: "Cells.CountLarge"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene el recuento total de objetos Cell instanciados"
type: docs
url: /es/net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Obtiene el recuento total de objetos Cell instanciados.

```csharp
public long CountLarge { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyCountLargeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B2"].PutValue("World");
            worksheet.Cells["C3"].PutValue(123);
            
            // Demostrar la propiedad CountLarge
            long cellCount = worksheet.Cells.CountLarge;
            Console.WriteLine($"Total cells in worksheet: {cellCount}");
            
            // Mostrar el tamaño de papel para la demostración
            Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
            Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


