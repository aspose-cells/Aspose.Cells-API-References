---
title: "DataBar.AxisPosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtiene o establece la posición del eje de las barras de datos especificadas por una regla de formato condicional"
type: docs
url: /es/net/aspose.cells/databar/axisposition/
---
## DataBar.AxisPosition property

Obtiene o establece la posición del eje de las barras de datos especificado por una regla de formato condicional.

```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisPositionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // Agregar formato condicional de barra de datos
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];
            
            // Configurar propiedades de la barra de datos
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            
            // Establecer posición del eje (demostración principal)
            cond.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
            cond.DataBar.AxisColor = Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("DataBarAxisPositionDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar with AxisPosition demo created successfully.");
        }
    }
}
```

### Ver también

* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


