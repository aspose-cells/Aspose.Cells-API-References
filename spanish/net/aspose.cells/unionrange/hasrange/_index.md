---
title: "UnionRange.HasRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Indica si esto tiene rango"
type: docs
url: /es/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Indica si esto tiene rango.

```csharp
public bool HasRange { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyHasRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un rango de unión usando la API correcta
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Verificar si el rango de unión tiene rangos válidos
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // Establecer valor y estilo solo si el rango es válido
            if (unionRange.HasRange)
            {
                unionRange.Value = "Test Value";
                
                Style style = workbook.CreateStyle();
                style.Pattern = BackgroundType.Solid;
                style.ForegroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });
            }
            
            workbook.Save("UnionRangeHasRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


