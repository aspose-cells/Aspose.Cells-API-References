---
title: "StyleFlag.DiagonalDownBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán los ajustes del borde diagonal descendente"
type: docs
url: /es/net/aspose.cells/styleflag/diagonaldownborder/
---
## StyleFlag.DiagonalDownBorder property

Se aplicarán las configuraciones de borde diagonal descendente.

```csharp
public bool DiagonalDownBorder { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalDownBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Down Border Demo");

            // Crear un objeto de estilo y establecer el borde diagonal descendente
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 0, 255);
            
            // Crear una bandera de estilo y habilitar la bandera de borde diagonal descendente
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalDownBorder = true;

            // Aplicar el estilo con la bandera a la celda
            cell.SetStyle(style, styleFlag);

            // Verificar si la bandera de borde diagonal descendente está habilitada
            Console.WriteLine("DiagonalDownBorder flag is enabled: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Deshabilitar la bandera de borde diagonal descendente
            styleFlag.DiagonalDownBorder = false;
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 255, 0);

            // Aplicar el estilo con la bandera a la celda
            cell.SetStyle(style, styleFlag);
            Console.WriteLine("DiagonalDownBorder flag is now: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Guarda el libro de trabajo
            workbook.Save("StyleFlagPropertyDiagonalDownBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


