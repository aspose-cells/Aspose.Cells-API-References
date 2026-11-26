---
title: "StyleFlag.RightBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán los ajustes del borde derecho"
type: docs
url: /es/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Se aplicarán las configuraciones de borde derecho.

```csharp
public bool RightBorder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con bordes
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // Crear una bandera de estilo y habilitar el borde derecho
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // Guarda el libro de trabajo
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


