---
title: "Range.Merge"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Combina un rango de celdas en una sola celda"
type: docs
url: /es/net/aspose.cells/range/merge/
---
## Range.Merge method

Combina un rango de celdas en una sola celda.

```csharp
public void Merge()
```

### Observaciones

Referencia la celda fusionada mediante la dirección de la celda superior izquierda del rango.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango y combinar celdas (3 filas x 2 columnas)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // Establecer valor en la celda combinada
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // Aplicar estilo a las celdas combinadas
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


