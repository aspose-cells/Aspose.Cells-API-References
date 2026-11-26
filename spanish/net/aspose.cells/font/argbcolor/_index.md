---
title: "Font.ArgbColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene y establece el color con un valor ARGB de 32 bits"
type: docs
url: /es/net/aspose.cells/font/argbcolor/
---
## Font.ArgbColor property

Obtiene y establece el color con un valor ARGB de 32 bits.

```csharp
public int ArgbColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a celdas y establecer valores con diferentes colores de fuente
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Red Text");
            Style style1 = cell1.GetStyle();
            style1.Font.ArgbColor = unchecked((int)0xFFFF0000); // Red
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Blue Text");
            Style style2 = cell2.GetStyle();
            style2.Font.ArgbColor = unchecked((int)0xFF0000FF); // Blue
            cell2.SetStyle(style2);

            Cell cell3 = worksheet.Cells["A3"];
            cell3.PutValue("Green Text");
            Style style3 = cell3.GetStyle();
            style3.Font.ArgbColor = unchecked((int)0xFF00FF00); // Green
            cell3.SetStyle(style3);

            // Verificar y mostrar los colores
            Console.WriteLine("Cell A1 Font Color: 0x{0:X8}", worksheet.Cells["A1"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A2 Font Color: 0x{0:X8}", worksheet.Cells["A2"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A3 Font Color: 0x{0:X8}", worksheet.Cells["A3"].GetStyle().Font.ArgbColor);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


