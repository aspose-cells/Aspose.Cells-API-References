---
title: "DataBar.BarFillType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtiene o establece cómo se rellena una barra de datos con color"
type: docs
url: /es/net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

Obtiene o establece cómo se rellena una barra de datos con color.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarFillTypeDemo
    {
        public static void Run()
        {
            // Instanciar un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establecer el rango del formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 5,
                StartColumn = 0,
                EndColumn = 5
            };
            fcs.AddArea(ca);

            // Agregar condición DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Configurar propiedades de DataBar
            DataBar dataBar = fc.DataBar;
            dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
            dataBar.Color = Color.Blue;

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);

            // Guarda el libro de trabajo
            workbook.Save("DataBarFillTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


