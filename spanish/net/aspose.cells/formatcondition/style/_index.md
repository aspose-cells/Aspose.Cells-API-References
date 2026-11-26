---
title: "FormatCondition.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtiene o establece el estilo de los rangos de celdas con formato condicional"
type: docs
url: /es/net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

Obtiene o establece el estilo de los rangos de celdas con formato condicional.

```csharp
public Style Style { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(30);
            worksheet.Cells["A2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(90);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establecer el rango
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            // Agregar primera condición (valores entre 40-80)
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "40", "80");
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Yellow;
            fc1.Style.Font.Color = System.Drawing.Color.Black;

            // Agregar segunda condición (valores > 80)
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "80", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;
            fc2.Style.Font.Color = System.Drawing.Color.White;
            fc2.Style.Font.IsBold = true;

            // Guarda el libro de trabajo
            workbook.Save("FormatConditionStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


