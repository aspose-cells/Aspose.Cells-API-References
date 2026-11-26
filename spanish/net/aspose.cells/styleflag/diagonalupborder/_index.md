---
title: "StyleFlag.DiagonalUpBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán los ajustes de borde diagonal ascendente"
type: docs
url: /es/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Se aplicarán las configuraciones de borde diagonal ascendente.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Cree un objeto de estilo y establezca el borde diagonal ascendente
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // Cree una bandera de estilo y habilite la bandera de borde diagonal ascendente
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Aplicar el estilo con la bandera a la celda
            cell.SetStyle(style, styleFlag);

            // Cree otra celda para demostrar el efecto
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Cree un estilo diferente para comparar
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // Aplique el segundo estilo con la misma bandera
            cell2.SetStyle(style2, styleFlag);

            // Guarda el libro de trabajo
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


