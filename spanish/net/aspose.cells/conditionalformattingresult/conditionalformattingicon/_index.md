---
title: "ConditionalFormattingResult.ConditionalFormattingIcon"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingResult. Obtiene la imagen del conjunto de íconos"
type: docs
url: /es/net/aspose.cells/conditionalformattingresult/conditionalformattingicon/
---
## ConditionalFormattingResult.ConditionalFormattingIcon property

Obtiene la imagen del conjunto de iconos.

```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingIconDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo y formato condicional
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Agregar formato condicional de conjunto de iconos
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Calcule fórmulas y obtenga el resultado del formato condicional
            workbook.CalculateFormula();
            ConditionalFormattingResult result = worksheet.Cells["A1"].GetConditionalFormattingResult();

            // Demuestre la propiedad ConditionalFormattingIcon
            if (result != null && result.ConditionalFormattingIcon != null)
            {
                Console.WriteLine("Icon Type: " + result.ConditionalFormattingIcon.Type);
                Console.WriteLine("Icon Index: " + result.ConditionalFormattingIcon.Index);
            }
        }
    }
}
```

### Ver también

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


