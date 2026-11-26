---
title: "DataBar.MaxCfvo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtiene o establece este objeto de valor máximo de DataBar. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Min en él"
type: docs
url: /es/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Obtener o establecer el objeto de valor máximo de esta DataBar. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Min en él.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
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

            // Agregar formato condicional de barra de datos
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Agregar barra de datos
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // Establecer valor MaxCfvo
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // Guarda el libro de trabajo
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


