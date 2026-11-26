---
title: "ColorFilter.GetColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ColorFilter. Obtiene el color de este filtro"
type: docs
url: /es/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Obtiene el color de este filtro.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hojas | WorksheetCollection |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // Cree filtro automático
            worksheet.AutoFilter.Range = "A1:A4";
            
            // Crear filtro de color
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // Obtener el filtro de color y verificar su color
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            if (colorFilter != null)
            {
                Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
                Console.WriteLine("Filter color: " + retrievedColor.ToString());
            }
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


