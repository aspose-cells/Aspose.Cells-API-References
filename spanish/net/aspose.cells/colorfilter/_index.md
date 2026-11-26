---
title: "Clase ColorFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ColorFilter. Representa la configuración para filtrar el rango por color"
type: docs
url: /es/net/aspose.cells/colorfilter/
---
## ColorFilter class

Representa la configuración para filtrar el rango por color.

```csharp
public class ColorFilter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FilterByFillColor](../../aspose.cells/colorfilter/filterbyfillcolor/) { get; set; } | Si filtrar por el color de relleno de la celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetColor](../../aspose.cells/colorfilter/getcolor/)(WorksheetCollection) | Obtiene el color de este filtro. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassColorFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra con diferentes colores
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Red");
            cells["A2"].PutValue("Green");
            cells["A3"].PutValue("Blue");
            cells["A4"].PutValue("Red");
            
            // Aplicar colores a las celdas
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A1"].SetStyle(style1);
            cells["A4"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Green;
            style2.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = Color.Blue;
            style3.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style3);
            
            // Cree filtro automático
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Crear filtro de color para celdas rojas
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, cr, cr);
            filter.Refresh();
            
            // Verificar filas filtradas
            Console.WriteLine("Row 1 hidden: " + cells.IsRowHidden(0));
            Console.WriteLine("Row 2 hidden: " + cells.IsRowHidden(1));
            Console.WriteLine("Row 3 hidden: " + cells.IsRowHidden(2));
            Console.WriteLine("Row 4 hidden: " + cells.IsRowHidden(3));
            
            // Acceder al filtro de color
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            Console.WriteLine("Filter by fill color: " + cf.FilterByFillColor);
            Console.WriteLine("Filter color: " + cf.GetColor(workbook.Worksheets));
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


