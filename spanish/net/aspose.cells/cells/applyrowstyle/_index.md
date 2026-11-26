---
title: "Cells.ApplyRowStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Aplica formatos a una fila completa"
type: docs
url: /es/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Aplica formatos a toda la fila.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| estilo | Estilo | El objeto de estilo que se aplicará. |
| bandera | StyleFlag | Banderas que indican las propiedades de formato aplicadas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un estilo con bordes
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Crear bandera de estilo para bordes
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Aplicar el estilo a la primera fila
            cells.ApplyRowStyle(0, style, styleFlag);

            // Guarda el libro de trabajo
            workbook.Save("ApplyRowStyleDemo.xlsx");
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


