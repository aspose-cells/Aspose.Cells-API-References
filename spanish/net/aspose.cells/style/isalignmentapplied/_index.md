---
title: "Style.IsAlignmentApplied"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si se debe aplicar el formato de alineación"
type: docs
url: /es/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

Indica si se debe aplicar el formato de alineación.

```csharp
public bool IsAlignmentApplied { get; set; }
```

### Observaciones

Solo para estilo con nombre.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsAlignmentAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            
            // Establece las propiedades de alineación
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // Habilita la aplicación de alineación
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // Verifica que la alineación se haya aplicado
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


