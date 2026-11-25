---
title: "Range.SetOutlineBorders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo"
type: docs
url: /it/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Imposta i bordi esterni attorno a un intervallo di celle con lo stesso stile e colore di bordo.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyle | CellBorderType | Stile del bordo. |
| borderColor | CellsColor | Colore del bordo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBordersWithCellBorderTypeCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea un oggetto CellsColor con un colore tematico
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Crea un intervallo e imposta i bordi di contorno
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Salva la cartella di lavoro
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Imposta i bordi esterni attorno a un intervallo di celle con lo stesso stile e colore di bordo.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyle | CellBorderType | Stile del bordo. |
| borderColor | Color | Colore del bordo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo di celle (A1:D4)
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Riempie l'intervallo con alcuni dati per rendere i bordi visibili
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // Chiama SetOutlineBorders con stile bordo medio e colore rosso
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // Salva la cartella di lavoro per vedere l'effetto
                workbook.Save("RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Imposta i bordi esterni attorno a un intervallo di celle.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Stili dei bordi. |
| borderColors | Color[] | Colori dei bordi. |

### Osservazioni

Sia la lunghezza di borderStyles che borderStyles deve essere 4. L'ordine di borderStyles e borderStyles deve essere top,bottom,left,right

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo di celle (B2:D4)
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // Prepara gli stili dei bordi e i colori
            CellBorderType[] borderStyles = new CellBorderType[]
            {
                CellBorderType.Thick,
                CellBorderType.Dashed,
                CellBorderType.Double,
                CellBorderType.MediumDashDot
            };

            Color[] borderColors = new Color[]
            {
                Color.Red,
                Color.Blue,
                Color.Green,
                Color.Purple
            };

            try
            {
                // Imposta i bordi di contorno con stili e colori diversi
                range.SetOutlineBorders(borderStyles, borderColors);

                // Riempie le celle con dati per rendere i bordi visibili
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RangeSetOutlineBordersDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


