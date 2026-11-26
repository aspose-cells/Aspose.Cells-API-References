---
title: "StyleFlag.LeftBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán los ajustes del borde izquierdo"
type: docs
url: /es/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Se aplicarán las configuraciones de borde izquierdo.

```csharp
public bool LeftBorder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Crear un rango y aplicar el estilo de borde izquierdo
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // Crear estilo y bandera
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // Establecer propiedades del borde izquierdo
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // Aplicar el estilo con la bandera de borde izquierdo
            range.ApplyStyle(style, flag);

            // Verificar que se aplicó el borde izquierdo
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // Guarda el libro de trabajo
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


