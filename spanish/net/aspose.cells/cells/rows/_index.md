---
title: "Cells.Rows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene la colección de objetos Row que representan las filas individuales en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/rows/
---
## Cells.Rows property

Obtiene la colección de objetos [`Row`](../../row/) que representan las filas individuales en esta hoja de cálculo.

```csharp
public RowCollection Rows { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establece el ancho de columna y la altura de fila
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // Accede a las propiedades de la fila a través de la colección Rows
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // Modifica las propiedades de la fila
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // Verificar cambios
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // Guarda el libro de trabajo
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


