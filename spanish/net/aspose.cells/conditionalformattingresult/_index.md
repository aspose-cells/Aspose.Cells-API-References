---
title: "Clase ConditionalFormattingResult"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ConditionalFormattingResult. Representa el resultado del formato condicional que se aplica a una celda"
type: docs
url: /es/net/aspose.cells/conditionalformattingresult/
---
## ConditionalFormattingResult class

Representa el resultado del formato condicional que se aplica a una celda.

```csharp
public class ConditionalFormattingResult
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ColorScaleResult](../../aspose.cells/conditionalformattingresult/colorscaleresult/) { get; } | Obtiene el color de visualización de la escala de colores. |
| [ConditionalFormattingColorScale](../../aspose.cells/conditionalformattingresult/conditionalformattingcolorscale/) { get; } | Obtiene el objeto ColorScale. |
| [ConditionalFormattingDataBar](../../aspose.cells/conditionalformattingresult/conditionalformattingdatabar/) { get; } | Obtiene el objeto DataBar. |
| [ConditionalFormattingIcon](../../aspose.cells/conditionalformattingresult/conditionalformattingicon/) { get; } | Obtiene la imagen del conjunto de iconos. |
| [ConditionalStyle](../../aspose.cells/conditionalformattingresult/conditionalstyle/) { get; } | Obtiene el estilo del resultado condicional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingResultDemo
    {
        public static void ConditionalFormattingResultExample()
        {
            // Instanciar un objeto de libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establece el rango de formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Agregar condición
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Establecer propiedades de ColorScale
            fc.ColorScale.Is3ColorScale = true;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxColor = Color.Green;

            // Aplicar algunos valores a las celdas
            for (int i = 0; i <= 10; i++)
            {
                for (int j = 0; j <= 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Obtener el resultado del formato condicional para una celda específica
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();

            // Acceder a las propiedades de ConditionalFormattingResult
            Style conditionalStyle = cfr.ConditionalStyle;
            ConditionalFormattingIcon icon = cfr.ConditionalFormattingIcon;
            DataBar dataBar = cfr.ConditionalFormattingDataBar;
            ColorScale colorScale = cfr.ConditionalFormattingColorScale;
            Color colorScaleResult = cfr.ColorScaleResult;

            // Mostrar algunas de las propiedades
            Console.WriteLine("Conditional Style Background Color: " + (conditionalStyle != null ? conditionalStyle.BackgroundColor : Color.Empty));
            Console.WriteLine("Conditional Formatting Icon Type: " + (icon != null ? icon.Type.ToString() : "No Icon"));
            Console.WriteLine("Conditional Formatting DataBar Color: " + (dataBar != null ? dataBar.Color.ToString() : "No DataBar"));
            Console.WriteLine("Conditional Formatting ColorScale Min Color: " + (colorScale != null ? colorScale.MinColor.ToString() : "No ColorScale"));
            Console.WriteLine("Color Scale Result: " + colorScaleResult);

            // Guarda el libro de trabajo
            workbook.Save("ConditionalFormattingResultExample.xlsx");
            workbook.Save("ConditionalFormattingResultExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


