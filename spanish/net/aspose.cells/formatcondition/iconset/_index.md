---
title: "FormatCondition.IconSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtenga la instancia IconSet del formato condicional. El tipo predeterminado de instancia IconSetType es TrafficLights31. Válido solo para el tipo IconSet"
type: docs
url: /es/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Obtenga la instancia "IconSet" del formato condicional. El IconSetType de la instancia predeterminada es TrafficLights31. Válido solo para type = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Agregar formato condicional
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Establecer el rango de celdas
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Agregar condición y establecer el tipo a IconSet
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Obtener el IconSet y configurarlo
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Guarda el libro de trabajo
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### Ver también

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


