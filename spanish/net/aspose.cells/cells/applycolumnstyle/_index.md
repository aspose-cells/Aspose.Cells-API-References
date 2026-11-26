---
title: "Cells.ApplyColumnStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Aplica formatos a toda una columna"
type: docs
url: /es/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Aplica formatos a toda una columna.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | El índice de columna. |
| estilo | Estilo | El objeto de estilo que se aplicará. |
| bandera | StyleFlag | Banderas que indican las propiedades de formato aplicadas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Crear un estilo con bordes
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Crear una bandera de estilo para aplicar solo bordes
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // Aplicar el estilo a la columna 1 (índice 0)
            cells.ApplyColumnStyle(0, style, sflag);

            // Guarda el libro de trabajo
            workbook.Save("ApplyColumnStyleOutput.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


