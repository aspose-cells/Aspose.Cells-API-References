---
title: "NegativeBarFormat.ColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NegativeBarFormat. Obtiene o establece si se debe usar el mismo color de relleno que las barras de datos positivas"
type: docs
url: /es/net/aspose.cells/negativebarformat/colortype/
---
## NegativeBarFormat.ColorType property

Obtiene o establece si se debe usar el mismo color de relleno que las barras de datos positivas.

```csharp
public DataBarNegativeColorType ColorType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-15);
            sheet.Cells["F4"].PutValue(25);
            sheet.Cells["G3"].PutValue(-5);
            sheet.Cells["G4"].PutValue(15);

            // Crear rango de formato condicional
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Agregar formato condicional de barra de datos
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(area);
            
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Establecer propiedades de la barra de datos
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            
            // Configurar formato de barra negativa
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("NegativeBarFormatDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved with negative bar formatting.");
        }
    }
}
```

### Ver también

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


