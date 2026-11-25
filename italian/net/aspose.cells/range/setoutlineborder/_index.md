---
title: "Range.SetOutlineBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Imposta il bordo di contorno attorno a un intervallo di celle"
type: docs
url: /it/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Imposta il bordo esterno attorno a un intervallo di celle.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderEdge | BorderType | Bordo esterno. |
| borderStyle | CellBorderType | Stile del bordo. |
| borderColor | CellsColor | Colore del bordo. |

### Esempi

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

            // Crea un oggetto CellsColor
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Crea un intervallo e imposta il bordo destro
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // Crea un altro intervallo e imposta tutti i bordi
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Salva la cartella di lavoro
            workbook.Save("SetOutlineBorderExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Imposta il bordo esterno attorno a un intervallo di celle.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderEdge | BorderType | Bordo esterno. |
| borderStyle | CellBorderType | Stile del bordo. |
| borderColor | Color | Colore del bordo. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo di celle
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // Imposta i bordi di contorno con diversi tipi di bordo e colori
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // Salva la cartella di lavoro
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


