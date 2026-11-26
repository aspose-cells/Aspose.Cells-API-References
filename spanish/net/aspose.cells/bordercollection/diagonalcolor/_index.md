---
title: "BorderCollection.DiagonalColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BorderCollection. Obtiene o establece el Color de las líneas diagonales"
type: docs
url: /es/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

Obtiene o establece el Color de las líneas diagonales.

```csharp
public Color DiagonalColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Border Demo");

            Style style = cell.GetStyle();
            
            // Configurando propiedades de borde diagonal
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


