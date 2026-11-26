---
title: "Enum CellBorderType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.CellBorderType enum. Enumera un tipo de borde de celda"
type: docs
url: /es/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

Enumera el tipo de borde de una celda.

```csharp
public enum CellBorderType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DashDot | `9` | Representa una línea delgada guion-punteada. |
| DashDotDot | `11` | Representa una línea delgada guion-punto-punteada. |
| Dashed | `3` | Representa una línea discontinua. |
| Dotted | `4` | Representa una línea punteada. |
| Double | `6` | Representa una línea doble. |
| Hair | `7` | Representa una línea delgada. |
| MediumDashDot | `10` | Representa una línea mediana guion-punteada. |
| MediumDashDotDot | `12` | Representa una línea mediana guion-punto-punteada. |
| MediumDashed | `8` | Representa una línea mediana discontinua. |
| None | `0` | Representa ninguna línea. |
| Medium | `2` | Representa una línea mediana. |
| SlantedDashDot | `13` | Representa una línea mediana guion-punteada inclinada. |
| Thick | `5` | Representa una línea gruesa. |
| Thin | `1` | Representa una línea delgada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Obtener el estilo del rango
            Style style = workbook.CreateStyle();

            // Establecer diferentes estilos de borde para el rango
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // Aplicar el estilo al rango
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // Guarda el libro de trabajo
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


