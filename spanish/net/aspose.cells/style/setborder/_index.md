---
title: "Style.SetBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Establece los bordes del estilo"
type: docs
url: /es/net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Establece los bordes del estilo.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderType | BorderType | El/los borde(s) a establecer pueden ser una combinación de [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | El estilo del borde. |
| borderColor | Color | El color del borde. |

### Valor de retorno

Si la configuración actual del borde ha sido modificada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            var range = worksheet.Cells.CreateRange("A1:D4");

            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            workbook.Save("BorderExample.xlsx");
        }
    }
}
```

### Ver también

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Establece los bordes del estilo.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderType | BorderType | El/los borde(s) a establecer pueden ser una combinación de [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | El estilo del borde. |
| borderColor | CellsColor | El color del borde. |

### Valor de retorno

Si la configuración actual del borde ha sido modificada.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // Crear un estilo
                Style style = workbook.CreateStyle();
                
                // Crear un objeto CellsColor usando el método de fábrica adecuado
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // Llamar a SetBorder con los parámetros BorderType, CellBorderType y CellsColor
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // Aplicar el estilo a una celda
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // Guarda el libro de trabajo
                workbook.Save("SetBorderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetBorder: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


