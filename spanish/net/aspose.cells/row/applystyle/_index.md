---
title: "Row.ApplyStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Aplica formatos para una fila completa"
type: docs
url: /es/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Aplica formatos a toda la fila.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El objeto de estilo que se aplicará. |
| bandera | StyleFlag | Banderas que indican las propiedades de formato aplicadas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer contenido HTML en la primera celda
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // Obtener la primera fila y su estilo
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // Modificar propiedades de estilo
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Aplicar estilo con banderas específicas (solo se aplicará el ajuste de texto)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // Ajuste automático para demostración
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // Guarda el libro de trabajo
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


