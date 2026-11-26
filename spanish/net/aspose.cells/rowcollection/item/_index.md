---
title: "RowCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RowCollection. Obtiene un objeto Row por el índice de fila dado. El objeto Row del índice de fila dado se instanciará si no existe previamente"
type: docs
url: /es/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Obtiene un objeto [`Row`](../../row/) por el índice de fila dado. El objeto Row del índice de fila dado se instanciará si no existe previamente.

```csharp
public Row this[int rowIndex] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer ancho estándar para columnas
            cells.StandardWidth = 20.0;

            // Acceder y dar estilo a filas usando la propiedad Item
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // Acceder y dar estilo a la celda en la fila
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // Guarda el libro de trabajo
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


