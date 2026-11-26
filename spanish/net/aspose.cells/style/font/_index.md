---
title: "Style.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene un objeto Font"
type: docs
url: /es/net/aspose.cells/style/font/
---
## Style.Font property

Obtiene un objeto `Font`.

```csharp
public Font Font { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Acceder a la celda B4 y establecer su fuente en negrita
            Cell b4 = cells["B4"];
            Style b4Style = b4.GetStyle();
            b4Style.Font.IsBold = true;
            b4.SetStyle(b4Style);

            // Acceder a la celda C4 y asegurar que su fuente no esté en negrita
            Cell c4 = cells["C4"];
            Style c4Style = c4.GetStyle();
            c4Style.Font.IsBold = false;
            c4.SetStyle(c4Style);

            // Acceder a la celda D4 y establecer su fuente en negrita con un color diferente
            Cell d4 = cells["D4"];
            Style d4Style = d4.GetStyle();
            d4Style.Font.IsBold = true;
            d4Style.Font.Color = Color.Red;
            d4.SetStyle(d4Style);

            // Verificar las propiedades de la fuente
            Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
            Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);

            // Guarda el libro de trabajo
            workbook.Save("FontPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


