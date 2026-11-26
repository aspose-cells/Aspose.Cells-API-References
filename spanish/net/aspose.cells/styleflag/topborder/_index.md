---
title: "StyleFlag.TopBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán los ajustes del borde superior"
type: docs
url: /es/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Se aplicarán las configuraciones de borde superior.

```csharp
public bool TopBorder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear un estilo con ajustes de borde superior
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // Crear una bandera de estilo y habilitar la modificación del borde superior
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // Aplicar el estilo a la celda A1 con solo la bandera de borde superior habilitada
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
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


