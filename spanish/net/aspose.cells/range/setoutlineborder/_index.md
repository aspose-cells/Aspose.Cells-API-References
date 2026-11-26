---
title: "Range.SetOutlineBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Establece un borde de contorno alrededor de un rango de celdas"
type: docs
url: /es/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Establece el borde exterior alrededor de un rango de celdas.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderEdge | BorderType | Borde del contorno. |
| borderStyle | CellBorderType | Estilo del borde. |
| borderColor | CellsColor | Color del borde. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un objeto CellsColor
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Crear un rango y establecer el borde derecho
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // Crear otro rango y establecer todos los bordes
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Guarda el libro de trabajo
            workbook.Save("SetOutlineBorderExample.xlsx");
        }
    }
}
```

### Ver también

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Establece el borde exterior alrededor de un rango de celdas.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderEdge | BorderType | Borde del contorno. |
| borderStyle | CellBorderType | Estilo del borde. |
| borderColor | Color | Color del borde. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango de celdas
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // Establecer bordes de contorno con diferentes tipos y colores de borde
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // Guarda el libro de trabajo
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


