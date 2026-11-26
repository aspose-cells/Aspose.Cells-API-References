---
title: "BorderCollection.DiagonalStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BorderCollection. Obtiene o establece el estilo de las líneas diagonales"
type: docs
url: /es/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Obtiene o establece el estilo de las líneas diagonales.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener una celda y su estilo
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Establecer propiedades del borde diagonal
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // Aplique el estilo a la celda
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


