---
title: "Style.Borders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene la BorderCollection del estilo"
type: docs
url: /es/net/aspose.cells/style/borders/
---
## Style.Borders property

Obtiene la [`BorderCollection`](../../bordercollection/) del estilo.

```csharp
public BorderCollection Borders { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener celda y su estilo
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Establecer diferentes estilos de borde
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // Aplique el estilo a la celda
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


