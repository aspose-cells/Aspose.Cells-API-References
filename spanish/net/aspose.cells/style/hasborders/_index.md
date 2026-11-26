---
title: "Style.HasBorders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Verifica si se han establecido bordes para el estilo"
type: docs
url: /es/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Comprueba si se han establecido bordes para el estilo.

```csharp
public bool HasBorders { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Acceder a la celda A1 y comprobar si tiene bordes (debería ser false por defecto)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // Crear un estilo con bordes
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Aplicar el estilo a la celda B1
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // Comprobar si la celda B1 tiene bordes (debería ser true ahora)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // Guarda el libro de trabajo
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


