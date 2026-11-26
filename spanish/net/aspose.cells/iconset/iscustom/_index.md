---
title: "IconSet.IsCustom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconSet. Indica si el conjunto de iconos es personalizado. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

Indica si el conjunto de íconos es personalizado. El valor predeterminado es false.

```csharp
public bool IsCustom { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Agregar formato condicional con un conjunto de iconos personalizado
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Establecer rango para formato condicional
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 9;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Agregar condición de conjunto de iconos
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Establecer el tipo de conjunto de iconos (usando un IconSetType válido)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Verificar la propiedad IsCustom (solo lectura)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


