---
title: "ConditionalFormattingResult.ConditionalStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingResult. Obtiene el estilo del resultado condicional"
type: docs
url: /es/net/aspose.cells/conditionalformattingresult/conditionalstyle/
---
## ConditionalFormattingResult.ConditionalStyle property

Obtiene el estilo del resultado condicional.

```csharp
public Style ConditionalStyle { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            
            // Cree una condición y establezca el estilo
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            fc.Style = style;

            // Obtenga la celda con formato condicional
            Cell cell = worksheet.Cells["A3"];
            Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
            
            // Muestre el color para demostrar la propiedad
            Console.WriteLine("Conditional Style Font Color: " + conditionalStyle.Font.Color);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


