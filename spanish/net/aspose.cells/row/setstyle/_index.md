---
title: "Row.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Establece el estilo de esta fila"
type: docs
url: /es/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

Establece el estilo de esta fila.

```csharp
public void SetStyle(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | el estilo que se usará como estilo predeterminado para las celdas en esta fila. |

### Observaciones

Este método solo establece el estilo dado como estilo predeterminado para esta fila, sin cambiar la configuración de estilo de las celdas existentes en esta fila. Para actualizar la configuración de estilo de las celdas existentes al estilo especificado al mismo tiempo, por favor use [`ApplyStyle`](../applystyle/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear y configurar un estilo
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // Obtener la primera fila y aplicar el estilo
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


