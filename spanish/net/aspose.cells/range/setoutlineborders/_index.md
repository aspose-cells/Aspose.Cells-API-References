---
title: "Range.SetOutlineBorders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Establece los bordes exteriores alrededor de un rango de celdas con el mismo estilo y color de borde"
type: docs
url: /es/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Establece los bordes exteriores alrededor de un rango de celdas con el mismo estilo y color de borde.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | CellBorderType | Estilo del borde. |
| borderColor | CellsColor | Color del borde. |

### Ejemplos

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

            // Crear un objeto CellsColor con un color de tema
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Crear un rango y establecer bordes exteriores
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Guarda el libro de trabajo
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Establece los bordes exteriores alrededor de un rango de celdas con el mismo estilo y color de borde.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | CellBorderType | Estilo del borde. |
| borderColor | Color | Color del borde. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango de celdas (A1:D4)
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Rellenar el rango con algunos datos para que los bordes sean visibles
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // Llamar a SetOutlineBorders con un estilo de borde medio y color rojo
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // Guardar el libro de trabajo para ver el efecto
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

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Establece bordes externos alrededor de un rango de celdas.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Estilos de borde. |
| borderColors | Color[] | Colores de borde. |

### Observaciones

Tanto la longitud de borderStyles como de borderStyles debe ser 4. El orden de borderStyles y borderStyles debe ser top,bottom,left,right

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango de celdas (B2:D4)
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // Preparar estilos de borde y colores
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
                // Establecer bordes exteriores con diferentes estilos y colores
                range.SetOutlineBorders(borderStyles, borderColors);

                // Rellenar celdas con datos para que los bordes sean visibles
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // Guarda el libro de trabajo
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

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


