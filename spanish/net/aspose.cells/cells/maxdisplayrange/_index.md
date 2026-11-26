---
title: "Cells.MaxDisplayRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene el rango máximo que incluye celdas fusionadas y formas"
type: docs
url: /es/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Obtiene el rango máximo que incluye datos, celdas combinadas y formas.

```csharp
public Range MaxDisplayRange { get; }
```

### Observaciones

Devuelve null si la hoja de cálculo está vacía desde Aspose.Cells 21.5.2.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos a las celdas para crear un rango de visualización
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Obtén el rango de visualización máximo
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // Muestra la información del rango
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // Crea un nuevo rango basado en las dimensiones del rango de visualización máximo
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // Aplica formato al rango
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Guarda el libro de trabajo
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


