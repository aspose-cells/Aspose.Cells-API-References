---
title: "UnionRange.SetOutlineBorders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnionRange. Establece bordes de contorno alrededor de un rango de celdas"
type: docs
url: /es/net/aspose.cells/unionrange/setoutlineborders/
---
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_1}

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
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeAColorArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Additional Data");

            // Crear un rango y convertirlo a UnionRange
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            UnionRange unionRange = worksheet.Cells.CreateRange(range.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range });

            try
            {
                // Definir estilos y colores de borde para los cuatro bordes
                CellBorderType[] borderStyles = new CellBorderType[]
                {
                    CellBorderType.Thin,    // Top border
                    CellBorderType.Medium,  // Right border
                    CellBorderType.Thick,   // Bottom border
                    CellBorderType.Double   // Left border
                };

                Color[] borderColors = new Color[]
                {
                    Color.Red,     // Top border color
                    Color.Blue,    // Right border color
                    Color.Green,   // Bottom border color
                    Color.Orange   // Left border color
                };

                // Llamar a SetOutlineBorders con los arreglos
                unionRange.SetOutlineBorders(borderStyles, borderColors);

                Console.WriteLine("SetOutlineBorders method called successfully with CellBorderType[] and Color[] parameters");
                Console.WriteLine($"Applied borders to range: {unionRange.RefersTo}");

                // Guarda el libro de trabajo
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders}

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
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test";
            worksheet.Cells["A2"].Value = "More Data";
            worksheet.Cells["B2"].Value = "Example";

            try
            {
                // Crea un UnionRange que cubra A1:B2
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Establecer bordes de contorno con un tipo de borde y color específicos
                unionRange.SetOutlineBorders(CellBorderType.Medium, Color.Blue);

                Console.WriteLine("SetOutlineBorders method called successfully");
                Console.WriteLine($"Border applied to range: {unionRange.RefersTo}");

                // Guarda el libro de trabajo
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


