---
title: "Border.LineStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Border. Obtiene o establece el tipo de borde de la celda"
type: docs
url: /es/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Obtiene o establece el tipo de borde de la celda.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a una celda y obtener su estilo
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Establecer diferentes estilos de línea de borde
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // Aplique el estilo a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


