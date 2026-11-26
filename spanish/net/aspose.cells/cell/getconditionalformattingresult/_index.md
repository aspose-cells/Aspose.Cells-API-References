---
title: "Cell.GetConditionalFormattingResult"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtenga el resultado del formato condicional"
type: docs
url: /es/net/aspose.cells/cell/getconditionalformattingresult/
---
## Cell.GetConditionalFormattingResult method

Obtén el resultado del formato condicional.

```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```

### Observaciones

Devuelve null si no se aplica formato condicional a esta celda,

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetConditionalFormattingResultDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            // Establecer condición y estilo
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fcc[conditionIndex].Style = style;

            // Obtener el resultado del formato condicional para una celda
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            // Resultado de salida
            Console.WriteLine("Cell A2 meets condition: " + (result.ConditionalStyle != null));
            Console.WriteLine("Applied font color: " + result.ConditionalStyle.Font.Color);
        }
    }
}
```

### Ver también

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


