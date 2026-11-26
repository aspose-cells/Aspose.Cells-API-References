---
title: "DataBar.MaxLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Representa la longitud máxima de la barra de datos"
type: docs
url: /es/net/aspose.cells/databar/maxlength/
---
## DataBar.MaxLength property

Representa la longitud máxima de la barra de datos.

```csharp
public int MaxLength { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            
            CellArea area = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(area);

            // Agregar barra de datos y establecer propiedades
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;
            
            dataBar.Color = Color.Blue;
            dataBar.MinLength = 0;
            dataBar.MaxLength = 90; // Demonstrating MaxLength property
            
            workbook.Save("DataBarMaxLengthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


