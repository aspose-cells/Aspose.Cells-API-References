---
title: "Cells.LastCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene la última celda en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Obtiene la última celda en esta hoja de cálculo.

```csharp
public Cell LastCell { get; }
```

### Observaciones

Devuelve null si no hay datos en la hoja de cálculo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyLastCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos
            worksheet.Cells["A1"].Value = "Header1";
            worksheet.Cells["B1"].Value = "Header2";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["B2"].Value = "Data2";

            // Obtener la dirección de la última celda
            Cell lastCell = worksheet.Cells.LastCell;
            Console.WriteLine("Last cell address: " + lastCell.Name);

            // Crear un rango desde la primera hasta la última celda
            Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
                worksheet.Cells.FirstCell.Name, 
                lastCell.Name);
            
            // Aplica formato al rango
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });

            // Guarda el libro de trabajo
            workbook.Save("LastCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


