---
title: "Font.IsStrikeout"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece un valor que indica si la fuente tiene tachado simple"
type: docs
url: /es/net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Obtiene o establece un valor que indica si la fuente tiene tachado simple.

```csharp
public bool IsStrikeout { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsStrikeoutDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Método 1: Establecer tachado a través del estilo directamente
            Cell cell1 = worksheet.Cells["A1"];
            Style style1 = cell1.GetStyle();
            style1.Font.IsStrikeout = true;
            cell1.SetStyle(style1);
            cell1.PutValue("Strikeout Text (Style)");
            
            // Método 2: Establecer tachado a través de HTML
            Cell cell2 = worksheet.Cells["A2"];
            cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
            
            // Verificar la propiedad de tachado
            Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
            Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
            
            // Guardar para verificación
            workbook.Save("FontStrikeoutDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


