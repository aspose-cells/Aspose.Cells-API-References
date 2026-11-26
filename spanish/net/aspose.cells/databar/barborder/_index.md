---
title: "DataBar.BarBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtiene un objeto que especifica el borde de una barra de datos"
type: docs
url: /es/net/aspose.cells/databar/barborder/
---
## DataBar.BarBorder property

Obtiene un objeto que especifica el borde de una barra de datos.

```csharp
public DataBarBorder BarBorder { get; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional de barra de datos
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Agregar condición de barra de datos
            int conditionIdx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIdx];

            // Establecer propiedades de la barra de datos
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            fc.DataBar.Color = Color.Blue;
            fc.DataBar.ShowValue = true;

            // Establecer propiedades del borde de la barra
            fc.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            fc.DataBar.BarBorder.Color = Color.Black;

            // Guarda el libro de trabajo
            workbook.Save("DataBarBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


