---
title: "Worksheet.ConditionalFormattings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene los ConditionalFormattings en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/conditionalformattings/
---
## Worksheet.ConditionalFormattings property

Obtiene los ConditionalFormattings en la hoja de cálculo.

```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyConditionalFormattingsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Crear formato condicional
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Establecer el rango
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Agregar condición
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


