---
title: "Cells.Columns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene la colección de objetos Column que representan las columnas individuales en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/columns/
---
## Cells.Columns property

Obtiene la colección de objetos [`Column`](../../column/) que representan las columnas individuales en esta hoja de cálculo.

```csharp
public ColumnCollection Columns { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer estilo para la columna 5
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // Establecer ancho para la columna 5
            cells.Columns[5].Width = 20;

            // Establecer datos en la columna 5 para demostrar el estilo
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


