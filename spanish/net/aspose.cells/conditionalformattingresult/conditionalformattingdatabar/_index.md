---
title: "ConditionalFormattingResult.ConditionalFormattingDataBar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingResult. Obtiene el objeto DataBar"
type: docs
url: /es/net/aspose.cells/conditionalformattingresult/conditionalformattingdatabar/
---
## ConditionalFormattingResult.ConditionalFormattingDataBar property

Obtiene el objeto DataBar.

```csharp
public DataBar ConditionalFormattingDataBar { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingDataBarDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue valores de muestra
            worksheet.Cells["A1"].PutValue(-6);
            worksheet.Cells["A2"].PutValue(-4);
            worksheet.Cells["A3"].PutValue(-2);
            worksheet.Cells["A4"].PutValue(0);
            worksheet.Cells["A5"].PutValue(2);
            worksheet.Cells["A6"].PutValue(4);
            worksheet.Cells["A7"].PutValue(6);

            // Agregar formato condicional de barra de datos
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 6;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcc[conditionIndex];
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            condition.DataBar.Color = System.Drawing.Color.Green;

            // Calcule fórmulas y aplique el formato
            workbook.CalculateFormula();

            // Obtenga el resultado del formato condicional y demuestre las propiedades de DataBar
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("DataBar Min Value: " + formattingResult.ConditionalFormattingDataBar.MinCfvo.Value);
            Console.WriteLine("DataBar Max Value: " + formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value);
            Console.WriteLine("DataBar Color: " + formattingResult.ConditionalFormattingDataBar.Color);
        }
    }
}
```

### Ver también

* class [DataBar](../../databar/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


