---
title: "Border.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Border. Obtiene o establece el Color del borde"
type: docs
url: /es/net/aspose.cells/border/color/
---
## Border.Color property

Obtiene o establece el color del borde.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderPropertyColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la celda A1
            Cell cell = worksheet.Cells["A1"];
            
            // Establecer el valor de la celda
            cell.PutValue("Border Color Demo");
            
            // Obtener el estilo de la celda
            Style style = cell.GetStyle();
            
            // Establecer colores y estilos del borde
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // Aplique el estilo a la celda
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### Ver también

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


