---
title: "ColorFilter.FilterByFillColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ColorFilter. Indica si filtrar por el color de relleno de las celdas"
type: docs
url: /es/net/aspose.cells/colorfilter/filterbyfillcolor/
---
## ColorFilter.FilterByFillColor property

Si filtrar por el color de relleno de la celda.

```csharp
public bool FilterByFillColor { get; set; }
```

### Observaciones

True: color de relleno de la celda; False: color de fuente de la celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterPropertyFilterByFillColorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de muestra con diferentes colores de relleno
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");

            // Establecer colores de relleno
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);

            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);

            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;

            // Crear filtro de color para el color de relleno
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, null);
            filter.Refresh();

            // Verificar la configuración del filtro
            FilterColumn filterColumn = filter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            // Demostrar la propiedad FilterByFillColor
            Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor); // Should be True
            Console.WriteLine("Filtered rows:");
            for (int row = 1; row <= 3; row++)
            {
                Console.WriteLine($"Row {row} hidden: {cells.IsRowHidden(row)}");
            }
        }
    }
}
```

### Ver también

* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


