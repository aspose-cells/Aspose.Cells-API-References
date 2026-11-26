---
title: "StyleFlag.BottomBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán los ajustes del borde inferior"
type: docs
url: /es/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

Se aplicarán las configuraciones del borde inferior.

```csharp
public bool BottomBorder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear un estilo con ajustes del borde inferior
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // Crear bandera de estilo y habilitar la modificación del borde inferior
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // Aplicar el estilo con la bandera a la celda A1
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
            cell.SetStyle(style, styleFlag);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


