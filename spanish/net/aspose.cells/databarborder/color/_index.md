---
title: "DataBarBorder.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad DataBarBorder. Obtiene o establece el color de los bordes de las barras de datos especificadas por una regla de formato condicional"
type: docs
url: /es/net/aspose.cells/databarborder/color/
---
## DataBarBorder.Color property

Obtiene o establece el color del borde de las barras de datos especificadas por una regla de formato condicional.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear una colección de condiciones de formato
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(new CellArea { StartRow = 2, StartColumn = 4, EndRow = 3, EndColumn = 6 });

            // Agregar condición de formato de barra de datos
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Establecer propiedades de la barra de datos
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Establecer propiedades del borde (demostrando el uso de Color)
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Guarda el libro de trabajo
            workbook.Save("DataBarBorderColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar border color demo completed.");
        }
    }
}
```

### Ver también

* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


