---
title: "DataBar.MinCfvo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtener o establecer este objeto de valor mínimo de la barra de datos. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Max en él"
type: docs
url: /es/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Obtener o establecer el objeto de valor mínimo de esta DataBar. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Max en él.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // Obtener la colección de formato condicional
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // Crear una barra de datos con MinCfvo establecido al tipo "Value"
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // Establecer el rango de la barra de datos
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Guarda el libro de trabajo
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


