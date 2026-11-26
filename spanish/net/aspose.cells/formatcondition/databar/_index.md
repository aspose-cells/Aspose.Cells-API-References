---
title: "FormatCondition.DataBar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtiene la instancia DataBar de los formatos condicionales. El color predeterminado de la instancia es azul. Válido solo para el tipo DataBar"
type: docs
url: /es/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Obtenga la instancia "DataBar" del formato condicional. El color de la instancia predeterminada es azul. Válido solo para type = DataBar.

```csharp
public DataBar DataBar { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Agregar formato condicional de barra de datos
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Establecer el rango para el formato condicional
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Agregar condición de barra de datos y establecer propiedades
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // Configurar propiedades de DataBar
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // Guarda el libro de trabajo
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### Ver también

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


