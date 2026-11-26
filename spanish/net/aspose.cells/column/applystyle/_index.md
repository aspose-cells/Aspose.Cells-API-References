---
title: "Column.ApplyStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Column. Aplica formatos a toda una columna"
type: docs
url: /es/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Aplica formatos a toda una columna.

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
    public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer texto multilínea en la columna 2
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // Crear estilo con ajuste de texto habilitado
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Aplicar estilo solo a la propiedad de ajuste de texto de la columna 2
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


