---
title: "Style.IsNumberFormatApplied"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si se debe aplicar el formato numérico"
type: docs
url: /es/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Indica si se debe aplicar el formato numérico.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Observaciones

Solo para estilo con nombre.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un estilo con formato numérico
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Verificar que el formato numérico se haya aplicado
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


